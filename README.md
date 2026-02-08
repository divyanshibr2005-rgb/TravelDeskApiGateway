# TravelDeskApiGateway
to add tests folder to the existing folder follow: 

create the tests folder where the TravelDeskApiGateway.slnx is with this :

``` dotnet new nunit -n TravelDeskApiGateway.Tests ```

then Add it to the solution:

```dotnet sln add TravelDeskApiGateway.Tests```

Reference the API Gateway project:

```dotnet add TravelDeskApiGateway.Tests reference TravelDeskApiGateway```

Install required packages:

```
cd TravelDeskApiGateway.Tests

dotnet add package Microsoft.AspNetCore.Mvc.Testing
dotnet add package FluentAssertions
```

then run:

```
dotnet build
dotnet test
```

