# Angular Azure Application Insights Sample

Demo Angular Integration with Azure Application Insights.
Build on top of Angular [Tour of Heroes App and Tutorial](https://angular.io/tutorial)

To configure just add your Application Insights instrumentation key to your ```C:\Sites\angular-sample\src\environments\environment.XXX.ts```

Note: Added ```src\environments\**``` files to ```.gitognore``` in this project to avoid storing into repository.    

```
export const environment = {
  production: true,
  appInsights: {

    instrumentationKey: '....'
    
    }
};

```   

## Sample Log Analytics Queries
Page Views:
```
pageViews
| where timestamp > ago(1d)
| sort by timestamp desc 
```

Traces:
```
traces
| where timestamp > ago(1d)
| sort by timestamp desc
``` 