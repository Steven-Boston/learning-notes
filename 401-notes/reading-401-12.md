# Reading 401-12: Entity Framework

## Microsoft Docs: Entity Framework Core
This documentation is available [here](https://docs.microsoft.com/en-us/ef/core/).

Entity Framework Core is a technology that allows for smooth accessing and management of data within .NET. It acheives this by making use of models, which in turn are built from classes (from classes? what a shock!). EF Core allows us to both handcraft a custom model for our database as well as handcraft a custom database from our model, and supports those delicious LINQ queries as well. 

## Microsoft Docs: Data Seeding
This documentation is available [here](https://docs.microsoft.com/en-us/ef/core/modeling/data-seeding).

Ever build a nice big database, but then run a general query to find nothing inside? You probably could stand to do some data seeding. The documentation lists three ways to get this done:

#### Model Seed Data

If we are prepared ahead of time, we can simply add seed data to our configuration when designing a model. The docs here provide a couple of options for snippets to add to the model's configuration, with prebuilt data within them. This can be a good option for getting some initial data setup, but won't be effective if the database/models are already running. It is also a bit finicky, requiring primary keys to be manually specified and being at risk of overwriting itself. As such, it is mostly useful for getting basic data that will not change and has few connections into the database. 

#### Manual Migration Customization

We can also directly add `.InsertData()`, `.UpdateData()`, and `DeleteData()` to the migration. This is much more straightforward, and the documentation simply provides this example: 

``` C#
migrationBuilder.InsertData(
    table: "Blogs",
    columns: new[] { "Url" },
    values: new object[] { "http://generated.com" });
```

#### Custom Initialization Logic

Custom Initialization Logic is a matter of providing some quantity of code that simply runs when the database initializes itself, whether by design or by simply removing it afterward. The Docs provide this example: 

``` C#
using (var context = new DataSeedingContext())
{
    context.Database.EnsureCreated();

    var testBlog = context.Blogs.FirstOrDefault(b => b.Url == "http://test.com");
    if (testBlog == null)
    {
        context.Blogs.Add(new Blog { Url = "http://test.com" });
    }

    context.SaveChanges();
}
```

## Code Fellows: User Secrets and Visual Studio
This documentation is available [here](https://codefellows.github.io/code-401-dotnet-guide/resources/user-secrets.html).

User secrets allows the intrepid developer to keep hidden those things which should not be transgressed. Like API keys and personal information and whatnot. To get this going, simply give a right-click to the project in Visual Studio and head to "manage user secrets". This summons to your aid a JSON file from another plane (the internet), within which you can place the critical details for safekeeping. 

Next, we'll need to get the .csproj on board. There should already be a `<UserSecretsId>` lurking about, but we'll also need to add in this little nugget:

`<DotNetCliToolReference Include="Microsoft.Extensions.SecretManager.Tools" Version="2.0.0" />`

With that, secrets are up and running. Next we will need to give the configuration files a mild overhaul (the appropriate code block is available in the article). This includes both a configuration block and an import. A quick controller construct and we will be able to access the secrets as needed with the proper keys. 

## MVS: Building Web APIs with ASP.NET Core 2.0
This video is available [here](https://www.youtube.com/watch?v=aIkpVzqLuhA).

## Microsoft Docs: Getting Started with EF Core
This tutorial is available [here](https://docs.microsoft.com/en-us/aspnet/core/data/ef-mvc/intro?view=aspnetcore-5.0).

## Microsoft Docs: Razor Pages with Entity Framework
This documentation is available [here](https://docs.microsoft.com/en-us/aspnet/core/data/ef-rp/intro?view=aspnetcore-2.1&tabs=visual-studio).


[<<Return to Home](../README.md)