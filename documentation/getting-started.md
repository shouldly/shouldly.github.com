# Getting Started with Shouldly

Shouldly can be [found here on NuGet](https://www.nuget.org/packages/Shouldly/) and can be installed by copying and pasting the following command into your Package Manager Console within Visual Studio (Tools > NuGet Package Manager > Package Manager Console).

```bash
Install-Package Shouldly
```

Alternatively if you're using .NET Core then you can install Shouldly via the command line interface with the following command:

```bash
dotnet add package Shouldly
```

## Your first Shouldly assertion

Once installed you're ready to try your first Shouldly assertion. To begin with we'll start with a simple string equality check. In a test method perform the following test:

```csharp
[Fact]
public void StringsShouldMatch()
{
    "hello world".ShouldBe("hello world");
}
```

This simple test should pass as it checks to ensure the string literal `hello world` (called the actual) is equivilent to the expected value.  
