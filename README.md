# Angular Azure Application Insights Sample

Demo Angular Integration with Azure Application Insights.

To configure just add your Application Insights instrumentation key to your ```C:\Sites\angular-sample\src\environments\environment.XXX.ts```

```
export const environment = {
  production: true,
  appInsights: {

    instrumentationKey: '....'
    
    }
};

```   