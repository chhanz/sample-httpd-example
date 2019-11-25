# OpenShift Source To Image Example (html source)
* * *
### Create new app
```bash
$ oc new-app httpd~https://github.com/chhanz/sample-httpd-example.git
```
   
```bash
$ oc new-app httpd~https://github.com/chhanz/sample-httpd-example.git
--> Found image 3413d55 (6 weeks old) in image stream "openshift/httpd" under tag "2.4" for "httpd"

    Apache httpd 2.4
    ----------------
    Apache httpd 2.4 available as container, is a powerful, efficient, and extensible web server. Apache supports a variety of features, many implemented as compiled modules which extend 
the core functionality. These can range from server-side programming language support to authentication schemes. Virtual hosting allows one Apache installation to serve many different Web sites.

    Tags: builder, httpd, httpd24

    * A source build using source code from https://github.com/chhanz/sample-httpd-example.git will be created
      * The resulting image will be pushed to image stream tag "sample-httpd-example:latest"
      * Use 'oc start-build' to trigger a new build
    * This image will be deployed in deployment config "sample-httpd-example"
    * Ports 8080/tcp, 8443/tcp will be load balanced by service "sample-httpd-example"
      * Other containers can access this service through the hostname "sample-httpd-example"

--> Creating resources ...
    imagestream.image.openshift.io "sample-httpd-example" created
    buildconfig.build.openshift.io "sample-httpd-example" created
    deploymentconfig.apps.openshift.io "sample-httpd-example" created
    service "sample-httpd-example" created
--> Success
    Build scheduled, use 'oc logs -f bc/sample-httpd-example' to track its progress.
    Application is not exposed. You can expose services to the outside world by executing one or more of the commands below:
     'oc expose svc/sample-httpd-example'
    Run 'oc status' to view your app.
```

### Use the Web Console
![create-app](https://chhanz.github.io/assets/images/post/2019-11-29-openshift-4/test1.png)
![create-app-2](https://chhanz.github.io/assets/images/post/2019-11-29-openshift-4/test2.png)
![create-app-3](https://chhanz.github.io/assets/images/post/2019-11-29-openshift-4/test3.png)
