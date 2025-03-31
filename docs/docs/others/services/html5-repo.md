If a `frontend` package is selected, the `mta.yaml` file will include `HTML5` repository configuration for the deployment of static files. On the other hand, if `XSUAA` is enabled, the `application` will retrieve static files from the HTML5 repository in a` protected mode`.

For `MTA` (Multi-Target Application) deployment, the `mta.yaml` file will contain the code for creating the `html5-repo` service as well.

```yaml
  - name: <app_name>-repo-runtime
    type: org.cloudfoundry.managed-service
    parameters:
      service-plan: app-runtime
      service: html5-apps-repo
  - name: <app_name>-repo-host
    type: org.cloudfoundry.managed-service
    parameters:
      service-plan: app-host
      service: html5-apps-repo
```