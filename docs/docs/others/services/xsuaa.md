Depending on whether XSUAA is selected, each package will have a distinct configuration in place to verify the JWT token and scopes of the incoming user if necessary. 

For further information on XSUAA, please refer to the following [link](https://sap.github.io/cloud-sdk/docs/java/guides/cloud-foundry-xsuaa-service)

For `MTA` (Multi-Target Application) deployment, the `mta.yaml` file will contain the code for creating the `XSUAA` service as well.

```yaml
- name: <app_name>-xsuaa
  type: org.cloudfoundry.managed-service
  parameters:
    service-plan: application
    service: xsuaa
    path: ./xs-security.json
```