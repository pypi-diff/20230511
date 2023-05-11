# Comparing `tmp/aws_prototyping_sdk.type_safe_api-0.18.5.tar.gz` & `tmp/aws_prototyping_sdk.type_safe_api-0.18.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_prototyping_sdk.type_safe_api-0.18.5.tar", last modified: Mon May  8 03:43:42 2023, max compression
+gzip compressed data, was "aws_prototyping_sdk.type_safe_api-0.18.6.tar", last modified: Thu May 11 05:07:43 2023, max compression
```

## Comparing `aws_prototyping_sdk.type_safe_api-0.18.5.tar` & `aws_prototyping_sdk.type_safe_api-0.18.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:43:42.329456 aws_prototyping_sdk.type_safe_api-0.18.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-08 03:43:30.000000 aws_prototyping_sdk.type_safe_api-0.18.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 03:43:30.000000 aws_prototyping_sdk.type_safe_api-0.18.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    61023 2023-05-08 03:43:42.329456 aws_prototyping_sdk.type_safe_api-0.18.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    60082 2023-05-08 03:43:30.000000 aws_prototyping_sdk.type_safe_api-0.18.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-08 03:43:30.000000 aws_prototyping_sdk.type_safe_api-0.18.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 03:43:42.329456 aws_prototyping_sdk.type_safe_api-0.18.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-08 03:43:30.000000 aws_prototyping_sdk.type_safe_api-0.18.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:43:42.313456 aws_prototyping_sdk.type_safe_api-0.18.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:43:42.313456 aws_prototyping_sdk.type_safe_api-0.18.5/src/aws_prototyping_sdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:43:42.317456 aws_prototyping_sdk.type_safe_api-0.18.5/src/aws_prototyping_sdk/type_safe_api/
--rw-r--r--   0 runner    (1001) docker     (123)   303094 2023-05-08 03:43:30.000000 aws_prototyping_sdk.type_safe_api-0.18.5/src/aws_prototyping_sdk/type_safe_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:43:42.329456 aws_prototyping_sdk.type_safe_api-0.18.5/src/aws_prototyping_sdk/type_safe_api/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-08 03:43:30.000000 aws_prototyping_sdk.type_safe_api-0.18.5/src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   878367 2023-05-08 03:43:30.000000 aws_prototyping_sdk.type_safe_api-0.18.5/src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.18.5.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 03:43:30.000000 aws_prototyping_sdk.type_safe_api-0.18.5/src/aws_prototyping_sdk/type_safe_api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:43:42.317456 aws_prototyping_sdk.type_safe_api-0.18.5/src/aws_prototyping_sdk.type_safe_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    61023 2023-05-08 03:43:42.000000 aws_prototyping_sdk.type_safe_api-0.18.5/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-08 03:43:42.000000 aws_prototyping_sdk.type_safe_api-0.18.5/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 03:43:42.000000 aws_prototyping_sdk.type_safe_api-0.18.5/src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-08 03:43:42.000000 aws_prototyping_sdk.type_safe_api-0.18.5/src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-08 03:43:42.000000 aws_prototyping_sdk.type_safe_api-0.18.5/src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:07:43.841022 aws_prototyping_sdk.type_safe_api-0.18.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-11 05:07:31.000000 aws_prototyping_sdk.type_safe_api-0.18.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 05:07:31.000000 aws_prototyping_sdk.type_safe_api-0.18.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    61480 2023-05-11 05:07:43.841022 aws_prototyping_sdk.type_safe_api-0.18.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    60539 2023-05-11 05:07:31.000000 aws_prototyping_sdk.type_safe_api-0.18.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-11 05:07:31.000000 aws_prototyping_sdk.type_safe_api-0.18.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 05:07:43.841022 aws_prototyping_sdk.type_safe_api-0.18.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-11 05:07:31.000000 aws_prototyping_sdk.type_safe_api-0.18.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:07:43.833022 aws_prototyping_sdk.type_safe_api-0.18.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:07:43.833022 aws_prototyping_sdk.type_safe_api-0.18.6/src/aws_prototyping_sdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:07:43.837022 aws_prototyping_sdk.type_safe_api-0.18.6/src/aws_prototyping_sdk/type_safe_api/
+-rw-r--r--   0 runner    (1001) docker     (123)   303551 2023-05-11 05:07:31.000000 aws_prototyping_sdk.type_safe_api-0.18.6/src/aws_prototyping_sdk/type_safe_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:07:43.837022 aws_prototyping_sdk.type_safe_api-0.18.6/src/aws_prototyping_sdk/type_safe_api/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-11 05:07:31.000000 aws_prototyping_sdk.type_safe_api-0.18.6/src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   879051 2023-05-11 05:07:31.000000 aws_prototyping_sdk.type_safe_api-0.18.6/src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.18.6.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 05:07:31.000000 aws_prototyping_sdk.type_safe_api-0.18.6/src/aws_prototyping_sdk/type_safe_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:07:43.837022 aws_prototyping_sdk.type_safe_api-0.18.6/src/aws_prototyping_sdk.type_safe_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    61480 2023-05-11 05:07:43.000000 aws_prototyping_sdk.type_safe_api-0.18.6/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-11 05:07:43.000000 aws_prototyping_sdk.type_safe_api-0.18.6/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 05:07:43.000000 aws_prototyping_sdk.type_safe_api-0.18.6/src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-11 05:07:43.000000 aws_prototyping_sdk.type_safe_api-0.18.6/src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 05:07:43.000000 aws_prototyping_sdk.type_safe_api-0.18.6/src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.5/LICENSE` & `aws_prototyping_sdk.type_safe_api-0.18.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.5/PKG-INFO` & `aws_prototyping_sdk.type_safe_api-0.18.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_prototyping_sdk.type_safe_api
-Version: 0.18.5
+Version: 0.18.6
 Summary: @aws-prototyping-sdk/type-safe-api
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -94,39 +94,41 @@
 ```
 
 #### Use the CDK Construct
 
 In your CDK application (ie within the `infra` project we created), consume the `Api` construct, vended from the generated typescript infrastructure package.
 
 ```python
-import { Stack, StackProps } from 'aws-cdk-lib';
-import { Construct } from 'constructs';
+import { Stack, StackProps } from "aws-cdk-lib";
+import { Construct } from "constructs";
 import { Api } from "myapi-typescript-infra"; // <- generated typescript infrastructure package
 import { Authorizers, Integrations } from "@aws-prototyping-sdk/type-safe-api";
 import { NodejsFunction } from "aws-cdk-lib/aws-lambda-nodejs";
 import { Cors } from "aws-cdk-lib/aws-apigateway";
-import * as path from 'path';
+import * as path from "path";
 
 export class MyStack extends Stack {
   constructor(scope: Construct, id: string, props: StackProps = {}) {
     super(scope, id, props);
 
     // Instantiate the generated CDK construct to deploy an API Gateway API based on your model
-    new Api(this, 'MyApi', {
+    new Api(this, "MyApi", {
       defaultAuthorizer: Authorizers.iam(),
       corsOptions: {
         allowOrigins: Cors.ALL_ORIGINS,
         allowMethods: Cors.ALL_METHODS,
       },
       // Supply an integration for every operation
       integrations: {
         sayHello: {
-          integration: Integrations.lambda(new NodejsFunction(this, 'SayHelloLambda', {
-            entry: path.resolve(__dirname, 'say-hello.ts'),
-          })),
+          integration: Integrations.lambda(
+            new NodejsFunction(this, "SayHelloLambda", {
+              entry: path.resolve(__dirname, "say-hello.ts"),
+            })
+          ),
         },
       },
     });
   }
 }
 ```
 
@@ -362,20 +364,20 @@
       parameters:
         - in: query
           name: name
           schema:
             type: string
           required: true
       responses:
-        '200':
+        "200":
           description: Successful response
           content:
-            'application/json':
+            "application/json":
               schema:
-                $ref: '#/components/schemas/HelloResponse'
+                $ref: "#/components/schemas/HelloResponse"
 components:
   schemas:
     HelloResponse:
       type: object
       properties:
         message:
           type: string
@@ -402,52 +404,52 @@
 
 ```yaml
 openapi: 3.0.3
 info:
   version: 1.0.0
   title: Example API
 paths:
-  $ref: './paths/index.yaml'
+  $ref: "./paths/index.yaml"
 components:
   schemas:
-    $ref: './schemas/index.yaml'
+    $ref: "./schemas/index.yaml"
 ```
 
 `paths/index.yaml`:
 
 ```yaml
 /hello:
   get:
-    $ref: './sayHello.yaml'
+    $ref: "./sayHello.yaml"
 ```
 
 `paths/sayHello.yaml`:
 
 ```yaml
 operationId: sayHello
 parameters:
- - in: query
-   name: name
-   schema:
-     type: string
-   required: true
+  - in: query
+    name: name
+    schema:
+      type: string
+    required: true
 responses:
-  '200':
+  "200":
     description: Successful response
     content:
-      'application/json':
+      "application/json":
         schema:
-          $ref: '../schemas/helloResponse.yaml'
+          $ref: "../schemas/helloResponse.yaml"
 ```
 
 `schemas/index.yaml`:
 
 ```yaml
 HelloResponse:
-  $ref: './helloResponse.yaml'
+  $ref: "./helloResponse.yaml"
 ```
 
 `schemas/helloResponse.yaml`:
 
 ```yaml
 type: object
 properties:
@@ -460,55 +462,57 @@
 ### Construct
 
 A CDK construct is generated in the `infrastructure/<language>` directory which provides a type-safe interface for creating an API Gateway API based on your model.
 
 You can extend or instantiate this construct in your CDK infrastructure project. You'll get a type error if you forget to define an integration for an operation defined in your api.
 
 ```python
-import { Authorizers, Integrations } from '@aws-prototyping-sdk/type-safe-api';
-import { NodejsFunction } from 'aws-cdk-lib/aws-lambda-nodejs';
-import { Construct } from 'constructs';
-import { Api } from 'myapi-typescript-infra';
+import { Authorizers, Integrations } from "@aws-prototyping-sdk/type-safe-api";
+import { NodejsFunction } from "aws-cdk-lib/aws-lambda-nodejs";
+import { Construct } from "constructs";
+import { Api } from "myapi-typescript-infra";
 
 /**
  * An example of how to wire lambda handler functions to the API
  */
 export class SampleApi extends Api {
   constructor(scope: Construct, id: string) {
     super(scope, id, {
       defaultAuthorizer: Authorizers.iam(),
       integrations: {
         // Every operation defined in your API must have an integration defined!
         sayHello: {
-          integration: Integrations.lambda(new NodejsFunction(scope, 'say-hello')),
+          integration: Integrations.lambda(
+            new NodejsFunction(scope, "say-hello")
+          ),
         },
       },
     });
   }
 }
 ```
 
 #### Sharing Integrations
 
 If you would like to use the same integration for every operation (for example you'd like to use a single lambda function to service all requests with the in-built [handler router](#handler-router)), you can use the `Operations.all` method from a generated runtime project to save repeating yourself:
 
 ```python
-import { Operations } from 'myapi-typescript-runtime';
-import { Authorizers, Integrations } from '@aws-prototyping-sdk/type-safe-api';
-import { NodejsFunction } from 'aws-cdk-lib/aws-lambda-nodejs';
-import { Construct } from 'constructs';
-import { Api } from 'myapi-typescript-infra';
+import { Operations } from "myapi-typescript-runtime";
+import { Authorizers, Integrations } from "@aws-prototyping-sdk/type-safe-api";
+import { NodejsFunction } from "aws-cdk-lib/aws-lambda-nodejs";
+import { Construct } from "constructs";
+import { Api } from "myapi-typescript-infra";
 
 export class SampleApi extends Api {
   constructor(scope: Construct, id: string) {
     super(scope, id, {
       defaultAuthorizer: Authorizers.iam(),
       // Use the same integration for every operation.
       integrations: Operations.all({
-        integration: Integrations.lambda(new NodejsFunction(scope, 'router')),
+        integration: Integrations.lambda(new NodejsFunction(scope, "router")),
       }),
     });
   }
 }
 ```
 
 TypeScript is demonstrated above, but this is also available in Java and Python.
@@ -526,29 +530,35 @@
 
 To use the Cognito authorizer, one or more user pools must be provided. You can optionally specify the scopes to check if using an access token. You can use the `withScopes` method to use the same authorizer but verify different scopes for individual integrations, for example:
 
 ```python
 export class SampleApi extends Api {
   constructor(scope: Construct, id: string) {
     const cognitoAuthorizer = Authorizers.cognito({
-      authorizerId: 'myCognitoAuthorizer',
-      userPools: [new UserPool(scope, 'UserPool')],
+      authorizerId: "myCognitoAuthorizer",
+      userPools: [new UserPool(scope, "UserPool")],
     });
 
     super(scope, id, {
       defaultAuthorizer: cognitoAuthorizer,
       integrations: {
         // Everyone in the user pool can call this operation:
         sayHello: {
-          integration: Integrations.lambda(new NodejsFunction(scope, 'say-hello')),
+          integration: Integrations.lambda(
+            new NodejsFunction(scope, "say-hello")
+          ),
         },
         // Only users with the given scopes can call this operation
         myRestrictedOperation: {
-          integration: Integrations.lambda(new NodejsFunction(scope, 'my-restricted-operation')),
-          authorizer: cognitoAuthorizer.withScopes('my-resource-server/my-scope'),
+          integration: Integrations.lambda(
+            new NodejsFunction(scope, "my-restricted-operation")
+          ),
+          authorizer: cognitoAuthorizer.withScopes(
+            "my-resource-server/my-scope"
+          ),
         },
       },
     });
   }
 }
 ```
 
@@ -558,27 +568,28 @@
 
 Custom authorizers use lambda functions to handle authorizing requests. These can either be simple token-based authorizers, or more complex request-based authorizers. See the [API Gateway documentation](https://docs.aws.amazon.com/apigateway/latest/developerguide/apigateway-use-lambda-authorizer.html) for more details.
 
 An example token-based authorizer (default):
 
 ```python
 Authorizers.custom({
-  authorizerId: 'myTokenAuthorizer',
-  function: new NodejsFunction(scope, 'authorizer'),
+  authorizerId: "myTokenAuthorizer",
+  function: new NodejsFunction(scope, "authorizer"),
 });
 ```
 
 An example request-based handler. By default the identitySource will be `method.request.header.Authorization`, however you can customise this as per [the API Gateway documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-apigateway-authorizer.html#cfn-apigateway-authorizer-identitysource).
 
 ```python
 Authorizers.custom({
-  authorizerId: 'myRequestAuthorizer',
+  authorizerId: "myRequestAuthorizer",
   type: CustomAuthorizerType.REQUEST,
-  identitySource: 'method.request.header.MyCustomHeader, method.request.querystring.myQueryString',
-  function: new NodejsFunction(scope, 'authorizer'),
+  identitySource:
+    "method.request.header.MyCustomHeader, method.request.querystring.myQueryString",
+  function: new NodejsFunction(scope, "authorizer"),
 });
 ```
 
 #### Integrations
 
 Integrations are used by API Gateway to service requests.
 
@@ -601,18 +612,20 @@
 The [typescript-fetch](https://openapi-generator.tech/docs/generators/typescript-fetch/) OpenAPI generator is used to generate typescript client. This requires an implementation of `fetch` to be passed to the client. In the browser one can pass the built in fetch, or in NodeJS you can use an implementation such as [node-fetch](https://www.npmjs.com/package/node-fetch).
 
 Example usage of the client in a website:
 
 ```python
 import { Configuration, DefaultApi } from "myapi-typescript-runtime";
 
-const client = new DefaultApi(new Configuration({
-  basePath: "https://xxxxxxxxxx.execute-api.ap-southeast-2.amazonaws.com",
-  fetchApi: window.fetch.bind(window),
-}));
+const client = new DefaultApi(
+  new Configuration({
+    basePath: "https://xxxxxxxxxx.execute-api.ap-southeast-2.amazonaws.com",
+    fetchApi: window.fetch.bind(window),
+  })
+);
 
 await client.sayHello({ name: "Jack" });
 ```
 
 #### Python
 
 The [python](https://openapi-generator.tech/docs/generators/python) OpenAPI generator is used to generate clients for python.
@@ -680,15 +693,19 @@
 ```
 
 ##### Handler Router
 
 The lambda handler wrappers can be used in isolation as handler methods for separate lambdas. If you would like to use a single lambda function to serve all requests, you can do so with the `handlerRouter`.
 
 ```python
-import { handlerRouter, sayHelloHandler, sayGoodbyeHandler } from "myapi-typescript-runtime";
+import {
+  handlerRouter,
+  sayHelloHandler,
+  sayGoodbyeHandler,
+} from "myapi-typescript-runtime";
 import { corsInterceptor } from "./interceptors";
 import { sayGoodbye } from "./handlers/say-goodbye";
 
 const sayHello = sayHelloHandler(async ({ input }) => {
   return {
     statusCode: 200,
     body: {
@@ -814,44 +831,65 @@
 import {
   sayHelloHandler,
   ChainedRequestInput,
   OperationResponse,
 } from "myapi-typescript-runtime";
 
 // Interceptor to wrap invocations in a try/catch, returning a 500 error for any unhandled exceptions.
-const tryCatchInterceptor = async <RequestParameters, RequestArrayParameters, RequestBody, Response>(
-  request: ChainedRequestInput<RequestParameters, RequestArrayParameters, RequestBody, Response>
+const tryCatchInterceptor = async <
+  RequestParameters,
+  RequestArrayParameters,
+  RequestBody,
+  Response
+>(
+  request: ChainedRequestInput<
+    RequestParameters,
+    RequestArrayParameters,
+    RequestBody,
+    Response
+  >
 ): Promise<Response | OperationResponse<500, { errorMessage: string }>> => {
   try {
     return await request.chain.next(request);
   } catch (e: any) {
-    return { statusCode: 500, body: { errorMessage: e.message }};
+    return { statusCode: 500, body: { errorMessage: e.message } };
   }
 };
 
 // tryCatchInterceptor is passed first, so it runs first and calls the second argument function (the request handler) via chain.next
-export const handler = sayHelloHandler(tryCatchInterceptor, async ({ input }) => {
-  return {
-    statusCode: 200,
-    body: {
-      message: `Hello ${input.requestParameters.name}!`,
-    },
-  };
-});
+export const handler = sayHelloHandler(
+  tryCatchInterceptor,
+  async ({ input }) => {
+    return {
+      statusCode: 200,
+      body: {
+        message: `Hello ${input.requestParameters.name}!`,
+      },
+    };
+  }
+);
 ```
 
 Another example interceptor might be to record request time metrics. The example below includes the full generic type signature for an interceptor:
 
 ```python
-import {
-  ChainedRequestInput,
-} from 'myapi-typescript-runtime';
+import { ChainedRequestInput } from "myapi-typescript-runtime";
 
-const timingInterceptor = async <RequestParameters, RequestArrayParameters, RequestBody, Response>(
-  request: ChainedRequestInput<RequestParameters, RequestArrayParameters, RequestBody, Response>
+const timingInterceptor = async <
+  RequestParameters,
+  RequestArrayParameters,
+  RequestBody,
+  Response
+>(
+  request: ChainedRequestInput<
+    RequestParameters,
+    RequestArrayParameters,
+    RequestBody,
+    Response
+  >
 ): Promise<Response> => {
   const start = Date.now();
   const response = await request.chain.next(request);
   const end = Date.now();
   console.log(`Took ${end - start} ms`);
   return response;
 };
@@ -859,18 +897,28 @@
 
 Interceptors may mutate the `interceptorContext` to pass state to further interceptors or the final lambda handler, for example an `identityInterceptor` might want to extract the authenticated user from the request so that it is available in handlers.
 
 ```python
 import {
   LambdaRequestParameters,
   LambdaHandlerChain,
-} from 'myapi-typescript-runtime';
+} from "myapi-typescript-runtime";
 
-const identityInterceptor = async <RequestParameters, RequestArrayParameters, RequestBody, Response>(
-  request: ChainedRequestInput<RequestParameters, RequestArrayParameters, RequestBody, Response>
+const identityInterceptor = async <
+  RequestParameters,
+  RequestArrayParameters,
+  RequestBody,
+  Response
+>(
+  request: ChainedRequestInput<
+    RequestParameters,
+    RequestArrayParameters,
+    RequestBody,
+    Response
+  >
 ): Promise<Response> => {
   const authenticatedUser = await getAuthenticatedUser(request.event);
   return await request.chain.next({
     ...request,
     interceptorContext: {
       ...request.interceptorContext,
       authenticatedUser,
@@ -1082,61 +1130,78 @@
 ```
 
 ##### Usage in a React Website
 
 First, make sure you create an instance of the API client (making sure to set the base URL and fetch instance). For example:
 
 ```python
-export const useMyApiClient = () => useMemo(() => new MyApi(new Configuration({
-  basePath: 'https://example123.execute-api.ap-southeast-2.amazonaws.com/prod',
-  fetchApi: window.fetch.bind(window),
-})), []);
+export const useMyApiClient = () =>
+  useMemo(
+    () =>
+      new MyApi(
+        new Configuration({
+          basePath:
+            "https://example123.execute-api.ap-southeast-2.amazonaws.com/prod",
+          fetchApi: window.fetch.bind(window),
+        })
+      ),
+    []
+  );
 ```
 
 Note that if you are using the [Cloudscape React Website](../cloudscape-react-ts-website/README.md) with [AWS NorthStar](https://aws.github.io/aws-northstar/) and IAM (Sigv4) Auth for your API, you can use NorthStar's [`useSigv4Client()` hook](https://aws.github.io/aws-northstar/?path=/story/components-cognitoauth-sigv4client-docs--page) to create
 an instance of `fetch` which will sign requests with the logged in user's credentials. For example:
 
 ```python
 export const useMyApiClient = () => {
-  const { client } = useSigv4Client();
-  return useMemo(() => client.current ? new MyApi(new Configuration({
-    basePath: 'https://example123.execute-api.ap-southeast-2.amazonaws.com/prod',
-    fetchApi: client.current,
-  })) : undefined, [client.current]);
+  const client = useSigv4Client();
+  return useMemo(
+    () =>
+      client
+        ? new MyApi(
+            new Configuration({
+              basePath:
+                "https://example123.execute-api.ap-southeast-2.amazonaws.com/prod",
+              fetchApi: client,
+            })
+          )
+        : undefined,
+    [client]
+  );
 };
 ```
 
 Next, instantiate the client provider above where you would like to use the hooks in your component hierarchy (such as above your router). For example:
 
 ```tsx
+import { DefaultApiClientProvider } from "myapi-typescript-react-query-hooks";
+
 const api = useMyApiClient();
 
 return api ? (
-  <MyApiClientContext.Provider value={api}>
-    { /* Components within the provider may make use of the hooks */ }
-  </MyApiClientContext.Provider>
-) : <p>Loading...</p>;
+  <DefaultApiClientProvider apiClient={api}>
+    {/* Components within the provider may make use of the hooks */}
+  </DefaultApiClientProvider>
+) : (
+  <p>Loading...</p>
+);
 ```
 
 Finally, you can import and use your generated hooks. For example:
 
 ```tsx
 export const MyComponent: FC<MyComponentProps> = () => {
-  const sayHello = useSayHello({ name: 'World' });
+  const sayHello = useSayHello({ name: "World" });
 
-  return (
-    sayHello.isLoading ? (
-      <p>Loading...</p>
-    ) : (
-      sayHello.isError ? (
-        <p>Error!</p>
-      ) : (
-        <h1>{sayHello.data.message}</h1>
-      )
-    )
+  return sayHello.isLoading ? (
+    <p>Loading...</p>
+  ) : sayHello.isError ? (
+    <p>Error!</p>
+  ) : (
+    <h1>{sayHello.data.message}</h1>
   );
 };
 ```
 
 ##### Paginated Operations
 
 You can generate `useInfiniteQuery` hooks instead of `useQuery` hooks for paginated API operations, by making use of the vendor extension `x-paginated` in your operation in the OpenAPI specification. You must specify both the `inputToken` and `outputToken`, which indicate the properties from the input and output used for pagination. For example in OpenAPI:
@@ -1216,77 +1281,83 @@
 import { NxMonorepoProject } from "@aws-prototyping-sdk/nx-monorepo";
 import { TypeSafeApiProject } from "@aws-prototyping-sdk/type-safe-api";
 import { AwsCdkTypeScriptApp } from "projen/lib/awscdk";
 import { PythonProject } from "projen/lib/python";
 
 // Create the monorepo
 const monorepo = new NxMonorepoProject({
-  name: 'monorepo',
+  name: "monorepo",
   defaultReleaseBranch: "main",
 });
 
 // Create the API project
 const api = new TypeSafeApiProject({
   name: "myapi",
   parent: monorepo,
-  outdir: 'packages/api',
+  outdir: "packages/api",
   // Smithy as the model language. You can also use ModelLanguage.OPENAPI
   model: {
     language: ModelLanguage.SMITHY,
     options: {
       smithy: {
         serviceName: {
-          namespace: 'com.mycompany',
-          serviceName: 'MyApi',
+          namespace: "com.mycompany",
+          serviceName: "MyApi",
         },
       },
     },
   },
   // Generate client and server types in TypeScript, Python, and Java
   runtime: {
     languages: [Language.TYPESCRIPT, Language.PYTHON, Language.JAVA],
   },
   // Generate CDK infrastructure in Python
   infrastructure: {
     language: Language.PYTHON,
   },
   // Generate HTML documentation
   documentation: {
-    formats: [DocumentationFormat.HTML_REDOC]
+    formats: [DocumentationFormat.HTML_REDOC],
   },
 });
 
 // Create a project for our lambda handlers written in python
 const lambdas = new PythonProject({
   name: "lambdas",
   parent: monorepo,
-  outdir: 'packages/lambdas',
+  outdir: "packages/lambdas",
   authorEmail: "me@example.com",
   authorName: "me",
   moduleName: "lambdas",
   version: "1.0.0",
   // Poetry is used to simplify local python dependencies
   poetry: true,
 });
 
 // Add a local dependency on the generated python runtime
 monorepo.addPythonPoetryDependency(lambdas, api.runtime.python!);
 
 // Add commands to the lambda project's package task to create a distributable which can be deployed to AWS Lambda
 lambdas.packageTask.exec(`mkdir -p lambda-dist && rm -rf lambda-dist/*`);
-lambdas.packageTask.exec(`cp -r ${lambdas.moduleName} lambda-dist/${lambdas.moduleName}`);
-lambdas.packageTask.exec(`poetry export --without-hashes --format=requirements.txt > lambda-dist/requirements.txt`);
-lambdas.packageTask.exec(`pip install -r lambda-dist/requirements.txt --target lambda-dist --upgrade`);
-lambdas.gitignore.addPatterns('lambda-dist');
+lambdas.packageTask.exec(
+  `cp -r ${lambdas.moduleName} lambda-dist/${lambdas.moduleName}`
+);
+lambdas.packageTask.exec(
+  `poetry export --without-hashes --format=requirements.txt > lambda-dist/requirements.txt`
+);
+lambdas.packageTask.exec(
+  `pip install -r lambda-dist/requirements.txt --target lambda-dist --upgrade`
+);
+lambdas.gitignore.addPatterns("lambda-dist");
 
 // Create a CDK infrastructure project
 const infra = new AwsCdkPythonApp({
   name: "infra",
   parent: monorepo,
-  outdir: 'packages/infra',
+  outdir: "packages/infra",
   authorEmail: "me@example.com",
   authorName: "me",
   cdkVersion: "2.0.0",
   moduleName: "infra",
   version: "1.0.0",
   poetry: true,
 });
@@ -1366,31 +1437,31 @@
 import { NxMonorepoProject } from "@aws-prototyping-sdk/nx-monorepo";
 import { TypeSafeApiProject } from "@aws-prototyping-sdk/type-safe-api";
 import { AwsCdkTypeScriptApp } from "projen/lib/awscdk";
 import { JavaProject } from "projen/lib/java";
 
 // Create the monorepo
 const monorepo = new NxMonorepoProject({
-  name: 'monorepo',
+  name: "monorepo",
   defaultReleaseBranch: "main",
 });
 
 // Create the API project
 const api = new TypeSafeApiProject({
   name: "myapi",
   parent: monorepo,
-  outdir: 'packages/api',
+  outdir: "packages/api",
   // Smithy as the model language. You can also use ModelLanguage.OPENAPI
   model: {
     language: ModelLanguage.SMITHY,
     options: {
       smithy: {
         serviceName: {
-          namespace: 'com.mycompany',
-          serviceName: 'MyApi',
+          namespace: "com.mycompany",
+          serviceName: "MyApi",
         },
       },
     },
   },
   // Generate client and server types in TypeScript, Python and Java
   runtime: {
     languages: [Language.TYPESCRIPT, Language.PYTHON, Language.JAVA],
@@ -1404,15 +1475,15 @@
     formats: [DocumentationFormat.HTML_REDOC],
   },
 });
 
 const lambdas = new JavaProject({
   name: "lambdas",
   parent: monorepo,
-  outdir: 'packages/lambdas',
+  outdir: "packages/lambdas",
   artifactId: "lambdas",
   groupId: "com.my.api",
   version: "1.0.0",
 });
 
 // The lambdas package needs a dependency on the generated java runtime
 monorepo.addJavaDependency(lambdas, api.runtime.java!);
@@ -1430,15 +1501,15 @@
     },
   ],
 });
 
 const infra = new AwsCdkJavaApp({
   name: "infra",
   parent: monorepo,
-  outdir: 'packages/infra',
+  outdir: "packages/infra",
   artifactId: "infra",
   groupId: "com.my.api",
   mainClass: "com.my.api.MyApp",
   version: "1.0.0",
   cdkVersion: "2.0.0",
 });
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.5/README.md` & `aws_prototyping_sdk.type_safe_api-0.18.6/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: aws-prototyping-sdk.type-safe-api
+Version: 0.18.6
+Summary: @aws-prototyping-sdk/type-safe-api
+Home-page: https://github.com/aws/aws-prototyping-sdk
+Author: AWS APJ COPE<apj-cope@amazon.com>
+License: Apache-2.0
+Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: JavaScript
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved
+Requires-Python: ~=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## Type Safe API
 
 Define your APIs using [Smithy](https://smithy.io/2.0/) or [OpenAPI v3](https://swagger.io/specification/), and leverage the power of generated client and server types, infrastructure, documentation, and automatic input validation!
 
 This package vends a projen project type which allows you to define an API using either [Smithy](https://smithy.io/2.0/) or [OpenAPI v3](https://swagger.io/specification/), and a construct which manages deploying this API in API Gateway, given an integration (eg a lambda) for every operation.
 
 The project will generate "runtime" projects from your API definition in your desired languages, which can be utilised both client side for interacting with your API, or server side for implementing your API. The project also generates a type-safe CDK construct which ensures an integration is provided for every API operation.
@@ -70,39 +94,41 @@
 ```
 
 #### Use the CDK Construct
 
 In your CDK application (ie within the `infra` project we created), consume the `Api` construct, vended from the generated typescript infrastructure package.
 
 ```python
-import { Stack, StackProps } from 'aws-cdk-lib';
-import { Construct } from 'constructs';
+import { Stack, StackProps } from "aws-cdk-lib";
+import { Construct } from "constructs";
 import { Api } from "myapi-typescript-infra"; // <- generated typescript infrastructure package
 import { Authorizers, Integrations } from "@aws-prototyping-sdk/type-safe-api";
 import { NodejsFunction } from "aws-cdk-lib/aws-lambda-nodejs";
 import { Cors } from "aws-cdk-lib/aws-apigateway";
-import * as path from 'path';
+import * as path from "path";
 
 export class MyStack extends Stack {
   constructor(scope: Construct, id: string, props: StackProps = {}) {
     super(scope, id, props);
 
     // Instantiate the generated CDK construct to deploy an API Gateway API based on your model
-    new Api(this, 'MyApi', {
+    new Api(this, "MyApi", {
       defaultAuthorizer: Authorizers.iam(),
       corsOptions: {
         allowOrigins: Cors.ALL_ORIGINS,
         allowMethods: Cors.ALL_METHODS,
       },
       // Supply an integration for every operation
       integrations: {
         sayHello: {
-          integration: Integrations.lambda(new NodejsFunction(this, 'SayHelloLambda', {
-            entry: path.resolve(__dirname, 'say-hello.ts'),
-          })),
+          integration: Integrations.lambda(
+            new NodejsFunction(this, "SayHelloLambda", {
+              entry: path.resolve(__dirname, "say-hello.ts"),
+            })
+          ),
         },
       },
     });
   }
 }
 ```
 
@@ -338,20 +364,20 @@
       parameters:
         - in: query
           name: name
           schema:
             type: string
           required: true
       responses:
-        '200':
+        "200":
           description: Successful response
           content:
-            'application/json':
+            "application/json":
               schema:
-                $ref: '#/components/schemas/HelloResponse'
+                $ref: "#/components/schemas/HelloResponse"
 components:
   schemas:
     HelloResponse:
       type: object
       properties:
         message:
           type: string
@@ -378,52 +404,52 @@
 
 ```yaml
 openapi: 3.0.3
 info:
   version: 1.0.0
   title: Example API
 paths:
-  $ref: './paths/index.yaml'
+  $ref: "./paths/index.yaml"
 components:
   schemas:
-    $ref: './schemas/index.yaml'
+    $ref: "./schemas/index.yaml"
 ```
 
 `paths/index.yaml`:
 
 ```yaml
 /hello:
   get:
-    $ref: './sayHello.yaml'
+    $ref: "./sayHello.yaml"
 ```
 
 `paths/sayHello.yaml`:
 
 ```yaml
 operationId: sayHello
 parameters:
- - in: query
-   name: name
-   schema:
-     type: string
-   required: true
+  - in: query
+    name: name
+    schema:
+      type: string
+    required: true
 responses:
-  '200':
+  "200":
     description: Successful response
     content:
-      'application/json':
+      "application/json":
         schema:
-          $ref: '../schemas/helloResponse.yaml'
+          $ref: "../schemas/helloResponse.yaml"
 ```
 
 `schemas/index.yaml`:
 
 ```yaml
 HelloResponse:
-  $ref: './helloResponse.yaml'
+  $ref: "./helloResponse.yaml"
 ```
 
 `schemas/helloResponse.yaml`:
 
 ```yaml
 type: object
 properties:
@@ -436,55 +462,57 @@
 ### Construct
 
 A CDK construct is generated in the `infrastructure/<language>` directory which provides a type-safe interface for creating an API Gateway API based on your model.
 
 You can extend or instantiate this construct in your CDK infrastructure project. You'll get a type error if you forget to define an integration for an operation defined in your api.
 
 ```python
-import { Authorizers, Integrations } from '@aws-prototyping-sdk/type-safe-api';
-import { NodejsFunction } from 'aws-cdk-lib/aws-lambda-nodejs';
-import { Construct } from 'constructs';
-import { Api } from 'myapi-typescript-infra';
+import { Authorizers, Integrations } from "@aws-prototyping-sdk/type-safe-api";
+import { NodejsFunction } from "aws-cdk-lib/aws-lambda-nodejs";
+import { Construct } from "constructs";
+import { Api } from "myapi-typescript-infra";
 
 /**
  * An example of how to wire lambda handler functions to the API
  */
 export class SampleApi extends Api {
   constructor(scope: Construct, id: string) {
     super(scope, id, {
       defaultAuthorizer: Authorizers.iam(),
       integrations: {
         // Every operation defined in your API must have an integration defined!
         sayHello: {
-          integration: Integrations.lambda(new NodejsFunction(scope, 'say-hello')),
+          integration: Integrations.lambda(
+            new NodejsFunction(scope, "say-hello")
+          ),
         },
       },
     });
   }
 }
 ```
 
 #### Sharing Integrations
 
 If you would like to use the same integration for every operation (for example you'd like to use a single lambda function to service all requests with the in-built [handler router](#handler-router)), you can use the `Operations.all` method from a generated runtime project to save repeating yourself:
 
 ```python
-import { Operations } from 'myapi-typescript-runtime';
-import { Authorizers, Integrations } from '@aws-prototyping-sdk/type-safe-api';
-import { NodejsFunction } from 'aws-cdk-lib/aws-lambda-nodejs';
-import { Construct } from 'constructs';
-import { Api } from 'myapi-typescript-infra';
+import { Operations } from "myapi-typescript-runtime";
+import { Authorizers, Integrations } from "@aws-prototyping-sdk/type-safe-api";
+import { NodejsFunction } from "aws-cdk-lib/aws-lambda-nodejs";
+import { Construct } from "constructs";
+import { Api } from "myapi-typescript-infra";
 
 export class SampleApi extends Api {
   constructor(scope: Construct, id: string) {
     super(scope, id, {
       defaultAuthorizer: Authorizers.iam(),
       // Use the same integration for every operation.
       integrations: Operations.all({
-        integration: Integrations.lambda(new NodejsFunction(scope, 'router')),
+        integration: Integrations.lambda(new NodejsFunction(scope, "router")),
       }),
     });
   }
 }
 ```
 
 TypeScript is demonstrated above, but this is also available in Java and Python.
@@ -502,29 +530,35 @@
 
 To use the Cognito authorizer, one or more user pools must be provided. You can optionally specify the scopes to check if using an access token. You can use the `withScopes` method to use the same authorizer but verify different scopes for individual integrations, for example:
 
 ```python
 export class SampleApi extends Api {
   constructor(scope: Construct, id: string) {
     const cognitoAuthorizer = Authorizers.cognito({
-      authorizerId: 'myCognitoAuthorizer',
-      userPools: [new UserPool(scope, 'UserPool')],
+      authorizerId: "myCognitoAuthorizer",
+      userPools: [new UserPool(scope, "UserPool")],
     });
 
     super(scope, id, {
       defaultAuthorizer: cognitoAuthorizer,
       integrations: {
         // Everyone in the user pool can call this operation:
         sayHello: {
-          integration: Integrations.lambda(new NodejsFunction(scope, 'say-hello')),
+          integration: Integrations.lambda(
+            new NodejsFunction(scope, "say-hello")
+          ),
         },
         // Only users with the given scopes can call this operation
         myRestrictedOperation: {
-          integration: Integrations.lambda(new NodejsFunction(scope, 'my-restricted-operation')),
-          authorizer: cognitoAuthorizer.withScopes('my-resource-server/my-scope'),
+          integration: Integrations.lambda(
+            new NodejsFunction(scope, "my-restricted-operation")
+          ),
+          authorizer: cognitoAuthorizer.withScopes(
+            "my-resource-server/my-scope"
+          ),
         },
       },
     });
   }
 }
 ```
 
@@ -534,27 +568,28 @@
 
 Custom authorizers use lambda functions to handle authorizing requests. These can either be simple token-based authorizers, or more complex request-based authorizers. See the [API Gateway documentation](https://docs.aws.amazon.com/apigateway/latest/developerguide/apigateway-use-lambda-authorizer.html) for more details.
 
 An example token-based authorizer (default):
 
 ```python
 Authorizers.custom({
-  authorizerId: 'myTokenAuthorizer',
-  function: new NodejsFunction(scope, 'authorizer'),
+  authorizerId: "myTokenAuthorizer",
+  function: new NodejsFunction(scope, "authorizer"),
 });
 ```
 
 An example request-based handler. By default the identitySource will be `method.request.header.Authorization`, however you can customise this as per [the API Gateway documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-apigateway-authorizer.html#cfn-apigateway-authorizer-identitysource).
 
 ```python
 Authorizers.custom({
-  authorizerId: 'myRequestAuthorizer',
+  authorizerId: "myRequestAuthorizer",
   type: CustomAuthorizerType.REQUEST,
-  identitySource: 'method.request.header.MyCustomHeader, method.request.querystring.myQueryString',
-  function: new NodejsFunction(scope, 'authorizer'),
+  identitySource:
+    "method.request.header.MyCustomHeader, method.request.querystring.myQueryString",
+  function: new NodejsFunction(scope, "authorizer"),
 });
 ```
 
 #### Integrations
 
 Integrations are used by API Gateway to service requests.
 
@@ -577,18 +612,20 @@
 The [typescript-fetch](https://openapi-generator.tech/docs/generators/typescript-fetch/) OpenAPI generator is used to generate typescript client. This requires an implementation of `fetch` to be passed to the client. In the browser one can pass the built in fetch, or in NodeJS you can use an implementation such as [node-fetch](https://www.npmjs.com/package/node-fetch).
 
 Example usage of the client in a website:
 
 ```python
 import { Configuration, DefaultApi } from "myapi-typescript-runtime";
 
-const client = new DefaultApi(new Configuration({
-  basePath: "https://xxxxxxxxxx.execute-api.ap-southeast-2.amazonaws.com",
-  fetchApi: window.fetch.bind(window),
-}));
+const client = new DefaultApi(
+  new Configuration({
+    basePath: "https://xxxxxxxxxx.execute-api.ap-southeast-2.amazonaws.com",
+    fetchApi: window.fetch.bind(window),
+  })
+);
 
 await client.sayHello({ name: "Jack" });
 ```
 
 #### Python
 
 The [python](https://openapi-generator.tech/docs/generators/python) OpenAPI generator is used to generate clients for python.
@@ -656,15 +693,19 @@
 ```
 
 ##### Handler Router
 
 The lambda handler wrappers can be used in isolation as handler methods for separate lambdas. If you would like to use a single lambda function to serve all requests, you can do so with the `handlerRouter`.
 
 ```python
-import { handlerRouter, sayHelloHandler, sayGoodbyeHandler } from "myapi-typescript-runtime";
+import {
+  handlerRouter,
+  sayHelloHandler,
+  sayGoodbyeHandler,
+} from "myapi-typescript-runtime";
 import { corsInterceptor } from "./interceptors";
 import { sayGoodbye } from "./handlers/say-goodbye";
 
 const sayHello = sayHelloHandler(async ({ input }) => {
   return {
     statusCode: 200,
     body: {
@@ -790,44 +831,65 @@
 import {
   sayHelloHandler,
   ChainedRequestInput,
   OperationResponse,
 } from "myapi-typescript-runtime";
 
 // Interceptor to wrap invocations in a try/catch, returning a 500 error for any unhandled exceptions.
-const tryCatchInterceptor = async <RequestParameters, RequestArrayParameters, RequestBody, Response>(
-  request: ChainedRequestInput<RequestParameters, RequestArrayParameters, RequestBody, Response>
+const tryCatchInterceptor = async <
+  RequestParameters,
+  RequestArrayParameters,
+  RequestBody,
+  Response
+>(
+  request: ChainedRequestInput<
+    RequestParameters,
+    RequestArrayParameters,
+    RequestBody,
+    Response
+  >
 ): Promise<Response | OperationResponse<500, { errorMessage: string }>> => {
   try {
     return await request.chain.next(request);
   } catch (e: any) {
-    return { statusCode: 500, body: { errorMessage: e.message }};
+    return { statusCode: 500, body: { errorMessage: e.message } };
   }
 };
 
 // tryCatchInterceptor is passed first, so it runs first and calls the second argument function (the request handler) via chain.next
-export const handler = sayHelloHandler(tryCatchInterceptor, async ({ input }) => {
-  return {
-    statusCode: 200,
-    body: {
-      message: `Hello ${input.requestParameters.name}!`,
-    },
-  };
-});
+export const handler = sayHelloHandler(
+  tryCatchInterceptor,
+  async ({ input }) => {
+    return {
+      statusCode: 200,
+      body: {
+        message: `Hello ${input.requestParameters.name}!`,
+      },
+    };
+  }
+);
 ```
 
 Another example interceptor might be to record request time metrics. The example below includes the full generic type signature for an interceptor:
 
 ```python
-import {
-  ChainedRequestInput,
-} from 'myapi-typescript-runtime';
+import { ChainedRequestInput } from "myapi-typescript-runtime";
 
-const timingInterceptor = async <RequestParameters, RequestArrayParameters, RequestBody, Response>(
-  request: ChainedRequestInput<RequestParameters, RequestArrayParameters, RequestBody, Response>
+const timingInterceptor = async <
+  RequestParameters,
+  RequestArrayParameters,
+  RequestBody,
+  Response
+>(
+  request: ChainedRequestInput<
+    RequestParameters,
+    RequestArrayParameters,
+    RequestBody,
+    Response
+  >
 ): Promise<Response> => {
   const start = Date.now();
   const response = await request.chain.next(request);
   const end = Date.now();
   console.log(`Took ${end - start} ms`);
   return response;
 };
@@ -835,18 +897,28 @@
 
 Interceptors may mutate the `interceptorContext` to pass state to further interceptors or the final lambda handler, for example an `identityInterceptor` might want to extract the authenticated user from the request so that it is available in handlers.
 
 ```python
 import {
   LambdaRequestParameters,
   LambdaHandlerChain,
-} from 'myapi-typescript-runtime';
+} from "myapi-typescript-runtime";
 
-const identityInterceptor = async <RequestParameters, RequestArrayParameters, RequestBody, Response>(
-  request: ChainedRequestInput<RequestParameters, RequestArrayParameters, RequestBody, Response>
+const identityInterceptor = async <
+  RequestParameters,
+  RequestArrayParameters,
+  RequestBody,
+  Response
+>(
+  request: ChainedRequestInput<
+    RequestParameters,
+    RequestArrayParameters,
+    RequestBody,
+    Response
+  >
 ): Promise<Response> => {
   const authenticatedUser = await getAuthenticatedUser(request.event);
   return await request.chain.next({
     ...request,
     interceptorContext: {
       ...request.interceptorContext,
       authenticatedUser,
@@ -1058,61 +1130,78 @@
 ```
 
 ##### Usage in a React Website
 
 First, make sure you create an instance of the API client (making sure to set the base URL and fetch instance). For example:
 
 ```python
-export const useMyApiClient = () => useMemo(() => new MyApi(new Configuration({
-  basePath: 'https://example123.execute-api.ap-southeast-2.amazonaws.com/prod',
-  fetchApi: window.fetch.bind(window),
-})), []);
+export const useMyApiClient = () =>
+  useMemo(
+    () =>
+      new MyApi(
+        new Configuration({
+          basePath:
+            "https://example123.execute-api.ap-southeast-2.amazonaws.com/prod",
+          fetchApi: window.fetch.bind(window),
+        })
+      ),
+    []
+  );
 ```
 
 Note that if you are using the [Cloudscape React Website](../cloudscape-react-ts-website/README.md) with [AWS NorthStar](https://aws.github.io/aws-northstar/) and IAM (Sigv4) Auth for your API, you can use NorthStar's [`useSigv4Client()` hook](https://aws.github.io/aws-northstar/?path=/story/components-cognitoauth-sigv4client-docs--page) to create
 an instance of `fetch` which will sign requests with the logged in user's credentials. For example:
 
 ```python
 export const useMyApiClient = () => {
-  const { client } = useSigv4Client();
-  return useMemo(() => client.current ? new MyApi(new Configuration({
-    basePath: 'https://example123.execute-api.ap-southeast-2.amazonaws.com/prod',
-    fetchApi: client.current,
-  })) : undefined, [client.current]);
+  const client = useSigv4Client();
+  return useMemo(
+    () =>
+      client
+        ? new MyApi(
+            new Configuration({
+              basePath:
+                "https://example123.execute-api.ap-southeast-2.amazonaws.com/prod",
+              fetchApi: client,
+            })
+          )
+        : undefined,
+    [client]
+  );
 };
 ```
 
 Next, instantiate the client provider above where you would like to use the hooks in your component hierarchy (such as above your router). For example:
 
 ```tsx
+import { DefaultApiClientProvider } from "myapi-typescript-react-query-hooks";
+
 const api = useMyApiClient();
 
 return api ? (
-  <MyApiClientContext.Provider value={api}>
-    { /* Components within the provider may make use of the hooks */ }
-  </MyApiClientContext.Provider>
-) : <p>Loading...</p>;
+  <DefaultApiClientProvider apiClient={api}>
+    {/* Components within the provider may make use of the hooks */}
+  </DefaultApiClientProvider>
+) : (
+  <p>Loading...</p>
+);
 ```
 
 Finally, you can import and use your generated hooks. For example:
 
 ```tsx
 export const MyComponent: FC<MyComponentProps> = () => {
-  const sayHello = useSayHello({ name: 'World' });
+  const sayHello = useSayHello({ name: "World" });
 
-  return (
-    sayHello.isLoading ? (
-      <p>Loading...</p>
-    ) : (
-      sayHello.isError ? (
-        <p>Error!</p>
-      ) : (
-        <h1>{sayHello.data.message}</h1>
-      )
-    )
+  return sayHello.isLoading ? (
+    <p>Loading...</p>
+  ) : sayHello.isError ? (
+    <p>Error!</p>
+  ) : (
+    <h1>{sayHello.data.message}</h1>
   );
 };
 ```
 
 ##### Paginated Operations
 
 You can generate `useInfiniteQuery` hooks instead of `useQuery` hooks for paginated API operations, by making use of the vendor extension `x-paginated` in your operation in the OpenAPI specification. You must specify both the `inputToken` and `outputToken`, which indicate the properties from the input and output used for pagination. For example in OpenAPI:
@@ -1192,77 +1281,83 @@
 import { NxMonorepoProject } from "@aws-prototyping-sdk/nx-monorepo";
 import { TypeSafeApiProject } from "@aws-prototyping-sdk/type-safe-api";
 import { AwsCdkTypeScriptApp } from "projen/lib/awscdk";
 import { PythonProject } from "projen/lib/python";
 
 // Create the monorepo
 const monorepo = new NxMonorepoProject({
-  name: 'monorepo',
+  name: "monorepo",
   defaultReleaseBranch: "main",
 });
 
 // Create the API project
 const api = new TypeSafeApiProject({
   name: "myapi",
   parent: monorepo,
-  outdir: 'packages/api',
+  outdir: "packages/api",
   // Smithy as the model language. You can also use ModelLanguage.OPENAPI
   model: {
     language: ModelLanguage.SMITHY,
     options: {
       smithy: {
         serviceName: {
-          namespace: 'com.mycompany',
-          serviceName: 'MyApi',
+          namespace: "com.mycompany",
+          serviceName: "MyApi",
         },
       },
     },
   },
   // Generate client and server types in TypeScript, Python, and Java
   runtime: {
     languages: [Language.TYPESCRIPT, Language.PYTHON, Language.JAVA],
   },
   // Generate CDK infrastructure in Python
   infrastructure: {
     language: Language.PYTHON,
   },
   // Generate HTML documentation
   documentation: {
-    formats: [DocumentationFormat.HTML_REDOC]
+    formats: [DocumentationFormat.HTML_REDOC],
   },
 });
 
 // Create a project for our lambda handlers written in python
 const lambdas = new PythonProject({
   name: "lambdas",
   parent: monorepo,
-  outdir: 'packages/lambdas',
+  outdir: "packages/lambdas",
   authorEmail: "me@example.com",
   authorName: "me",
   moduleName: "lambdas",
   version: "1.0.0",
   // Poetry is used to simplify local python dependencies
   poetry: true,
 });
 
 // Add a local dependency on the generated python runtime
 monorepo.addPythonPoetryDependency(lambdas, api.runtime.python!);
 
 // Add commands to the lambda project's package task to create a distributable which can be deployed to AWS Lambda
 lambdas.packageTask.exec(`mkdir -p lambda-dist && rm -rf lambda-dist/*`);
-lambdas.packageTask.exec(`cp -r ${lambdas.moduleName} lambda-dist/${lambdas.moduleName}`);
-lambdas.packageTask.exec(`poetry export --without-hashes --format=requirements.txt > lambda-dist/requirements.txt`);
-lambdas.packageTask.exec(`pip install -r lambda-dist/requirements.txt --target lambda-dist --upgrade`);
-lambdas.gitignore.addPatterns('lambda-dist');
+lambdas.packageTask.exec(
+  `cp -r ${lambdas.moduleName} lambda-dist/${lambdas.moduleName}`
+);
+lambdas.packageTask.exec(
+  `poetry export --without-hashes --format=requirements.txt > lambda-dist/requirements.txt`
+);
+lambdas.packageTask.exec(
+  `pip install -r lambda-dist/requirements.txt --target lambda-dist --upgrade`
+);
+lambdas.gitignore.addPatterns("lambda-dist");
 
 // Create a CDK infrastructure project
 const infra = new AwsCdkPythonApp({
   name: "infra",
   parent: monorepo,
-  outdir: 'packages/infra',
+  outdir: "packages/infra",
   authorEmail: "me@example.com",
   authorName: "me",
   cdkVersion: "2.0.0",
   moduleName: "infra",
   version: "1.0.0",
   poetry: true,
 });
@@ -1342,31 +1437,31 @@
 import { NxMonorepoProject } from "@aws-prototyping-sdk/nx-monorepo";
 import { TypeSafeApiProject } from "@aws-prototyping-sdk/type-safe-api";
 import { AwsCdkTypeScriptApp } from "projen/lib/awscdk";
 import { JavaProject } from "projen/lib/java";
 
 // Create the monorepo
 const monorepo = new NxMonorepoProject({
-  name: 'monorepo',
+  name: "monorepo",
   defaultReleaseBranch: "main",
 });
 
 // Create the API project
 const api = new TypeSafeApiProject({
   name: "myapi",
   parent: monorepo,
-  outdir: 'packages/api',
+  outdir: "packages/api",
   // Smithy as the model language. You can also use ModelLanguage.OPENAPI
   model: {
     language: ModelLanguage.SMITHY,
     options: {
       smithy: {
         serviceName: {
-          namespace: 'com.mycompany',
-          serviceName: 'MyApi',
+          namespace: "com.mycompany",
+          serviceName: "MyApi",
         },
       },
     },
   },
   // Generate client and server types in TypeScript, Python and Java
   runtime: {
     languages: [Language.TYPESCRIPT, Language.PYTHON, Language.JAVA],
@@ -1380,15 +1475,15 @@
     formats: [DocumentationFormat.HTML_REDOC],
   },
 });
 
 const lambdas = new JavaProject({
   name: "lambdas",
   parent: monorepo,
-  outdir: 'packages/lambdas',
+  outdir: "packages/lambdas",
   artifactId: "lambdas",
   groupId: "com.my.api",
   version: "1.0.0",
 });
 
 // The lambdas package needs a dependency on the generated java runtime
 monorepo.addJavaDependency(lambdas, api.runtime.java!);
@@ -1406,15 +1501,15 @@
     },
   ],
 });
 
 const infra = new AwsCdkJavaApp({
   name: "infra",
   parent: monorepo,
-  outdir: 'packages/infra',
+  outdir: "packages/infra",
   artifactId: "infra",
   groupId: "com.my.api",
   mainClass: "com.my.api.MyApp",
   version: "1.0.0",
   cdkVersion: "2.0.0",
 });
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.5/setup.py` & `aws_prototyping_sdk.type_safe_api-0.18.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws_prototyping_sdk.type_safe_api",
-    "version": "0.18.5",
+    "version": "0.18.6",
     "description": "@aws-prototyping-sdk/type-safe-api",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-prototyping-sdk",
     "long_description_content_type": "text/markdown",
     "author": "AWS APJ COPE<apj-cope@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "aws_prototyping_sdk.type_safe_api",
         "aws_prototyping_sdk.type_safe_api._jsii"
     ],
     "package_data": {
         "aws_prototyping_sdk.type_safe_api._jsii": [
-            "type-safe-api@0.18.5.jsii.tgz"
+            "type-safe-api@0.18.6.jsii.tgz"
         ],
         "aws_prototyping_sdk.type_safe_api": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.5/src/aws_prototyping_sdk/type_safe_api/__init__.py` & `aws_prototyping_sdk.type_safe_api-0.18.6/src/aws_prototyping_sdk/type_safe_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,39 +71,41 @@
 ```
 
 #### Use the CDK Construct
 
 In your CDK application (ie within the `infra` project we created), consume the `Api` construct, vended from the generated typescript infrastructure package.
 
 ```python
-import { Stack, StackProps } from 'aws-cdk-lib';
-import { Construct } from 'constructs';
+import { Stack, StackProps } from "aws-cdk-lib";
+import { Construct } from "constructs";
 import { Api } from "myapi-typescript-infra"; // <- generated typescript infrastructure package
 import { Authorizers, Integrations } from "@aws-prototyping-sdk/type-safe-api";
 import { NodejsFunction } from "aws-cdk-lib/aws-lambda-nodejs";
 import { Cors } from "aws-cdk-lib/aws-apigateway";
-import * as path from 'path';
+import * as path from "path";
 
 export class MyStack extends Stack {
   constructor(scope: Construct, id: string, props: StackProps = {}) {
     super(scope, id, props);
 
     // Instantiate the generated CDK construct to deploy an API Gateway API based on your model
-    new Api(this, 'MyApi', {
+    new Api(this, "MyApi", {
       defaultAuthorizer: Authorizers.iam(),
       corsOptions: {
         allowOrigins: Cors.ALL_ORIGINS,
         allowMethods: Cors.ALL_METHODS,
       },
       // Supply an integration for every operation
       integrations: {
         sayHello: {
-          integration: Integrations.lambda(new NodejsFunction(this, 'SayHelloLambda', {
-            entry: path.resolve(__dirname, 'say-hello.ts'),
-          })),
+          integration: Integrations.lambda(
+            new NodejsFunction(this, "SayHelloLambda", {
+              entry: path.resolve(__dirname, "say-hello.ts"),
+            })
+          ),
         },
       },
     });
   }
 }
 ```
 
@@ -339,20 +341,20 @@
       parameters:
         - in: query
           name: name
           schema:
             type: string
           required: true
       responses:
-        '200':
+        "200":
           description: Successful response
           content:
-            'application/json':
+            "application/json":
               schema:
-                $ref: '#/components/schemas/HelloResponse'
+                $ref: "#/components/schemas/HelloResponse"
 components:
   schemas:
     HelloResponse:
       type: object
       properties:
         message:
           type: string
@@ -379,52 +381,52 @@
 
 ```yaml
 openapi: 3.0.3
 info:
   version: 1.0.0
   title: Example API
 paths:
-  $ref: './paths/index.yaml'
+  $ref: "./paths/index.yaml"
 components:
   schemas:
-    $ref: './schemas/index.yaml'
+    $ref: "./schemas/index.yaml"
 ```
 
 `paths/index.yaml`:
 
 ```yaml
 /hello:
   get:
-    $ref: './sayHello.yaml'
+    $ref: "./sayHello.yaml"
 ```
 
 `paths/sayHello.yaml`:
 
 ```yaml
 operationId: sayHello
 parameters:
- - in: query
-   name: name
-   schema:
-     type: string
-   required: true
+  - in: query
+    name: name
+    schema:
+      type: string
+    required: true
 responses:
-  '200':
+  "200":
     description: Successful response
     content:
-      'application/json':
+      "application/json":
         schema:
-          $ref: '../schemas/helloResponse.yaml'
+          $ref: "../schemas/helloResponse.yaml"
 ```
 
 `schemas/index.yaml`:
 
 ```yaml
 HelloResponse:
-  $ref: './helloResponse.yaml'
+  $ref: "./helloResponse.yaml"
 ```
 
 `schemas/helloResponse.yaml`:
 
 ```yaml
 type: object
 properties:
@@ -437,55 +439,57 @@
 ### Construct
 
 A CDK construct is generated in the `infrastructure/<language>` directory which provides a type-safe interface for creating an API Gateway API based on your model.
 
 You can extend or instantiate this construct in your CDK infrastructure project. You'll get a type error if you forget to define an integration for an operation defined in your api.
 
 ```python
-import { Authorizers, Integrations } from '@aws-prototyping-sdk/type-safe-api';
-import { NodejsFunction } from 'aws-cdk-lib/aws-lambda-nodejs';
-import { Construct } from 'constructs';
-import { Api } from 'myapi-typescript-infra';
+import { Authorizers, Integrations } from "@aws-prototyping-sdk/type-safe-api";
+import { NodejsFunction } from "aws-cdk-lib/aws-lambda-nodejs";
+import { Construct } from "constructs";
+import { Api } from "myapi-typescript-infra";
 
 /**
  * An example of how to wire lambda handler functions to the API
  */
 export class SampleApi extends Api {
   constructor(scope: Construct, id: string) {
     super(scope, id, {
       defaultAuthorizer: Authorizers.iam(),
       integrations: {
         // Every operation defined in your API must have an integration defined!
         sayHello: {
-          integration: Integrations.lambda(new NodejsFunction(scope, 'say-hello')),
+          integration: Integrations.lambda(
+            new NodejsFunction(scope, "say-hello")
+          ),
         },
       },
     });
   }
 }
 ```
 
 #### Sharing Integrations
 
 If you would like to use the same integration for every operation (for example you'd like to use a single lambda function to service all requests with the in-built [handler router](#handler-router)), you can use the `Operations.all` method from a generated runtime project to save repeating yourself:
 
 ```python
-import { Operations } from 'myapi-typescript-runtime';
-import { Authorizers, Integrations } from '@aws-prototyping-sdk/type-safe-api';
-import { NodejsFunction } from 'aws-cdk-lib/aws-lambda-nodejs';
-import { Construct } from 'constructs';
-import { Api } from 'myapi-typescript-infra';
+import { Operations } from "myapi-typescript-runtime";
+import { Authorizers, Integrations } from "@aws-prototyping-sdk/type-safe-api";
+import { NodejsFunction } from "aws-cdk-lib/aws-lambda-nodejs";
+import { Construct } from "constructs";
+import { Api } from "myapi-typescript-infra";
 
 export class SampleApi extends Api {
   constructor(scope: Construct, id: string) {
     super(scope, id, {
       defaultAuthorizer: Authorizers.iam(),
       // Use the same integration for every operation.
       integrations: Operations.all({
-        integration: Integrations.lambda(new NodejsFunction(scope, 'router')),
+        integration: Integrations.lambda(new NodejsFunction(scope, "router")),
       }),
     });
   }
 }
 ```
 
 TypeScript is demonstrated above, but this is also available in Java and Python.
@@ -503,29 +507,35 @@
 
 To use the Cognito authorizer, one or more user pools must be provided. You can optionally specify the scopes to check if using an access token. You can use the `withScopes` method to use the same authorizer but verify different scopes for individual integrations, for example:
 
 ```python
 export class SampleApi extends Api {
   constructor(scope: Construct, id: string) {
     const cognitoAuthorizer = Authorizers.cognito({
-      authorizerId: 'myCognitoAuthorizer',
-      userPools: [new UserPool(scope, 'UserPool')],
+      authorizerId: "myCognitoAuthorizer",
+      userPools: [new UserPool(scope, "UserPool")],
     });
 
     super(scope, id, {
       defaultAuthorizer: cognitoAuthorizer,
       integrations: {
         // Everyone in the user pool can call this operation:
         sayHello: {
-          integration: Integrations.lambda(new NodejsFunction(scope, 'say-hello')),
+          integration: Integrations.lambda(
+            new NodejsFunction(scope, "say-hello")
+          ),
         },
         // Only users with the given scopes can call this operation
         myRestrictedOperation: {
-          integration: Integrations.lambda(new NodejsFunction(scope, 'my-restricted-operation')),
-          authorizer: cognitoAuthorizer.withScopes('my-resource-server/my-scope'),
+          integration: Integrations.lambda(
+            new NodejsFunction(scope, "my-restricted-operation")
+          ),
+          authorizer: cognitoAuthorizer.withScopes(
+            "my-resource-server/my-scope"
+          ),
         },
       },
     });
   }
 }
 ```
 
@@ -535,27 +545,28 @@
 
 Custom authorizers use lambda functions to handle authorizing requests. These can either be simple token-based authorizers, or more complex request-based authorizers. See the [API Gateway documentation](https://docs.aws.amazon.com/apigateway/latest/developerguide/apigateway-use-lambda-authorizer.html) for more details.
 
 An example token-based authorizer (default):
 
 ```python
 Authorizers.custom({
-  authorizerId: 'myTokenAuthorizer',
-  function: new NodejsFunction(scope, 'authorizer'),
+  authorizerId: "myTokenAuthorizer",
+  function: new NodejsFunction(scope, "authorizer"),
 });
 ```
 
 An example request-based handler. By default the identitySource will be `method.request.header.Authorization`, however you can customise this as per [the API Gateway documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-apigateway-authorizer.html#cfn-apigateway-authorizer-identitysource).
 
 ```python
 Authorizers.custom({
-  authorizerId: 'myRequestAuthorizer',
+  authorizerId: "myRequestAuthorizer",
   type: CustomAuthorizerType.REQUEST,
-  identitySource: 'method.request.header.MyCustomHeader, method.request.querystring.myQueryString',
-  function: new NodejsFunction(scope, 'authorizer'),
+  identitySource:
+    "method.request.header.MyCustomHeader, method.request.querystring.myQueryString",
+  function: new NodejsFunction(scope, "authorizer"),
 });
 ```
 
 #### Integrations
 
 Integrations are used by API Gateway to service requests.
 
@@ -578,18 +589,20 @@
 The [typescript-fetch](https://openapi-generator.tech/docs/generators/typescript-fetch/) OpenAPI generator is used to generate typescript client. This requires an implementation of `fetch` to be passed to the client. In the browser one can pass the built in fetch, or in NodeJS you can use an implementation such as [node-fetch](https://www.npmjs.com/package/node-fetch).
 
 Example usage of the client in a website:
 
 ```python
 import { Configuration, DefaultApi } from "myapi-typescript-runtime";
 
-const client = new DefaultApi(new Configuration({
-  basePath: "https://xxxxxxxxxx.execute-api.ap-southeast-2.amazonaws.com",
-  fetchApi: window.fetch.bind(window),
-}));
+const client = new DefaultApi(
+  new Configuration({
+    basePath: "https://xxxxxxxxxx.execute-api.ap-southeast-2.amazonaws.com",
+    fetchApi: window.fetch.bind(window),
+  })
+);
 
 await client.sayHello({ name: "Jack" });
 ```
 
 #### Python
 
 The [python](https://openapi-generator.tech/docs/generators/python) OpenAPI generator is used to generate clients for python.
@@ -657,15 +670,19 @@
 ```
 
 ##### Handler Router
 
 The lambda handler wrappers can be used in isolation as handler methods for separate lambdas. If you would like to use a single lambda function to serve all requests, you can do so with the `handlerRouter`.
 
 ```python
-import { handlerRouter, sayHelloHandler, sayGoodbyeHandler } from "myapi-typescript-runtime";
+import {
+  handlerRouter,
+  sayHelloHandler,
+  sayGoodbyeHandler,
+} from "myapi-typescript-runtime";
 import { corsInterceptor } from "./interceptors";
 import { sayGoodbye } from "./handlers/say-goodbye";
 
 const sayHello = sayHelloHandler(async ({ input }) => {
   return {
     statusCode: 200,
     body: {
@@ -791,44 +808,65 @@
 import {
   sayHelloHandler,
   ChainedRequestInput,
   OperationResponse,
 } from "myapi-typescript-runtime";
 
 // Interceptor to wrap invocations in a try/catch, returning a 500 error for any unhandled exceptions.
-const tryCatchInterceptor = async <RequestParameters, RequestArrayParameters, RequestBody, Response>(
-  request: ChainedRequestInput<RequestParameters, RequestArrayParameters, RequestBody, Response>
+const tryCatchInterceptor = async <
+  RequestParameters,
+  RequestArrayParameters,
+  RequestBody,
+  Response
+>(
+  request: ChainedRequestInput<
+    RequestParameters,
+    RequestArrayParameters,
+    RequestBody,
+    Response
+  >
 ): Promise<Response | OperationResponse<500, { errorMessage: string }>> => {
   try {
     return await request.chain.next(request);
   } catch (e: any) {
-    return { statusCode: 500, body: { errorMessage: e.message }};
+    return { statusCode: 500, body: { errorMessage: e.message } };
   }
 };
 
 // tryCatchInterceptor is passed first, so it runs first and calls the second argument function (the request handler) via chain.next
-export const handler = sayHelloHandler(tryCatchInterceptor, async ({ input }) => {
-  return {
-    statusCode: 200,
-    body: {
-      message: `Hello ${input.requestParameters.name}!`,
-    },
-  };
-});
+export const handler = sayHelloHandler(
+  tryCatchInterceptor,
+  async ({ input }) => {
+    return {
+      statusCode: 200,
+      body: {
+        message: `Hello ${input.requestParameters.name}!`,
+      },
+    };
+  }
+);
 ```
 
 Another example interceptor might be to record request time metrics. The example below includes the full generic type signature for an interceptor:
 
 ```python
-import {
-  ChainedRequestInput,
-} from 'myapi-typescript-runtime';
+import { ChainedRequestInput } from "myapi-typescript-runtime";
 
-const timingInterceptor = async <RequestParameters, RequestArrayParameters, RequestBody, Response>(
-  request: ChainedRequestInput<RequestParameters, RequestArrayParameters, RequestBody, Response>
+const timingInterceptor = async <
+  RequestParameters,
+  RequestArrayParameters,
+  RequestBody,
+  Response
+>(
+  request: ChainedRequestInput<
+    RequestParameters,
+    RequestArrayParameters,
+    RequestBody,
+    Response
+  >
 ): Promise<Response> => {
   const start = Date.now();
   const response = await request.chain.next(request);
   const end = Date.now();
   console.log(`Took ${end - start} ms`);
   return response;
 };
@@ -836,18 +874,28 @@
 
 Interceptors may mutate the `interceptorContext` to pass state to further interceptors or the final lambda handler, for example an `identityInterceptor` might want to extract the authenticated user from the request so that it is available in handlers.
 
 ```python
 import {
   LambdaRequestParameters,
   LambdaHandlerChain,
-} from 'myapi-typescript-runtime';
+} from "myapi-typescript-runtime";
 
-const identityInterceptor = async <RequestParameters, RequestArrayParameters, RequestBody, Response>(
-  request: ChainedRequestInput<RequestParameters, RequestArrayParameters, RequestBody, Response>
+const identityInterceptor = async <
+  RequestParameters,
+  RequestArrayParameters,
+  RequestBody,
+  Response
+>(
+  request: ChainedRequestInput<
+    RequestParameters,
+    RequestArrayParameters,
+    RequestBody,
+    Response
+  >
 ): Promise<Response> => {
   const authenticatedUser = await getAuthenticatedUser(request.event);
   return await request.chain.next({
     ...request,
     interceptorContext: {
       ...request.interceptorContext,
       authenticatedUser,
@@ -1059,61 +1107,78 @@
 ```
 
 ##### Usage in a React Website
 
 First, make sure you create an instance of the API client (making sure to set the base URL and fetch instance). For example:
 
 ```python
-export const useMyApiClient = () => useMemo(() => new MyApi(new Configuration({
-  basePath: 'https://example123.execute-api.ap-southeast-2.amazonaws.com/prod',
-  fetchApi: window.fetch.bind(window),
-})), []);
+export const useMyApiClient = () =>
+  useMemo(
+    () =>
+      new MyApi(
+        new Configuration({
+          basePath:
+            "https://example123.execute-api.ap-southeast-2.amazonaws.com/prod",
+          fetchApi: window.fetch.bind(window),
+        })
+      ),
+    []
+  );
 ```
 
 Note that if you are using the [Cloudscape React Website](../cloudscape-react-ts-website/README.md) with [AWS NorthStar](https://aws.github.io/aws-northstar/) and IAM (Sigv4) Auth for your API, you can use NorthStar's [`useSigv4Client()` hook](https://aws.github.io/aws-northstar/?path=/story/components-cognitoauth-sigv4client-docs--page) to create
 an instance of `fetch` which will sign requests with the logged in user's credentials. For example:
 
 ```python
 export const useMyApiClient = () => {
-  const { client } = useSigv4Client();
-  return useMemo(() => client.current ? new MyApi(new Configuration({
-    basePath: 'https://example123.execute-api.ap-southeast-2.amazonaws.com/prod',
-    fetchApi: client.current,
-  })) : undefined, [client.current]);
+  const client = useSigv4Client();
+  return useMemo(
+    () =>
+      client
+        ? new MyApi(
+            new Configuration({
+              basePath:
+                "https://example123.execute-api.ap-southeast-2.amazonaws.com/prod",
+              fetchApi: client,
+            })
+          )
+        : undefined,
+    [client]
+  );
 };
 ```
 
 Next, instantiate the client provider above where you would like to use the hooks in your component hierarchy (such as above your router). For example:
 
 ```tsx
+import { DefaultApiClientProvider } from "myapi-typescript-react-query-hooks";
+
 const api = useMyApiClient();
 
 return api ? (
-  <MyApiClientContext.Provider value={api}>
-    { /* Components within the provider may make use of the hooks */ }
-  </MyApiClientContext.Provider>
-) : <p>Loading...</p>;
+  <DefaultApiClientProvider apiClient={api}>
+    {/* Components within the provider may make use of the hooks */}
+  </DefaultApiClientProvider>
+) : (
+  <p>Loading...</p>
+);
 ```
 
 Finally, you can import and use your generated hooks. For example:
 
 ```tsx
 export const MyComponent: FC<MyComponentProps> = () => {
-  const sayHello = useSayHello({ name: 'World' });
+  const sayHello = useSayHello({ name: "World" });
 
-  return (
-    sayHello.isLoading ? (
-      <p>Loading...</p>
-    ) : (
-      sayHello.isError ? (
-        <p>Error!</p>
-      ) : (
-        <h1>{sayHello.data.message}</h1>
-      )
-    )
+  return sayHello.isLoading ? (
+    <p>Loading...</p>
+  ) : sayHello.isError ? (
+    <p>Error!</p>
+  ) : (
+    <h1>{sayHello.data.message}</h1>
   );
 };
 ```
 
 ##### Paginated Operations
 
 You can generate `useInfiniteQuery` hooks instead of `useQuery` hooks for paginated API operations, by making use of the vendor extension `x-paginated` in your operation in the OpenAPI specification. You must specify both the `inputToken` and `outputToken`, which indicate the properties from the input and output used for pagination. For example in OpenAPI:
@@ -1193,77 +1258,83 @@
 import { NxMonorepoProject } from "@aws-prototyping-sdk/nx-monorepo";
 import { TypeSafeApiProject } from "@aws-prototyping-sdk/type-safe-api";
 import { AwsCdkTypeScriptApp } from "projen/lib/awscdk";
 import { PythonProject } from "projen/lib/python";
 
 // Create the monorepo
 const monorepo = new NxMonorepoProject({
-  name: 'monorepo',
+  name: "monorepo",
   defaultReleaseBranch: "main",
 });
 
 // Create the API project
 const api = new TypeSafeApiProject({
   name: "myapi",
   parent: monorepo,
-  outdir: 'packages/api',
+  outdir: "packages/api",
   // Smithy as the model language. You can also use ModelLanguage.OPENAPI
   model: {
     language: ModelLanguage.SMITHY,
     options: {
       smithy: {
         serviceName: {
-          namespace: 'com.mycompany',
-          serviceName: 'MyApi',
+          namespace: "com.mycompany",
+          serviceName: "MyApi",
         },
       },
     },
   },
   // Generate client and server types in TypeScript, Python, and Java
   runtime: {
     languages: [Language.TYPESCRIPT, Language.PYTHON, Language.JAVA],
   },
   // Generate CDK infrastructure in Python
   infrastructure: {
     language: Language.PYTHON,
   },
   // Generate HTML documentation
   documentation: {
-    formats: [DocumentationFormat.HTML_REDOC]
+    formats: [DocumentationFormat.HTML_REDOC],
   },
 });
 
 // Create a project for our lambda handlers written in python
 const lambdas = new PythonProject({
   name: "lambdas",
   parent: monorepo,
-  outdir: 'packages/lambdas',
+  outdir: "packages/lambdas",
   authorEmail: "me@example.com",
   authorName: "me",
   moduleName: "lambdas",
   version: "1.0.0",
   // Poetry is used to simplify local python dependencies
   poetry: true,
 });
 
 // Add a local dependency on the generated python runtime
 monorepo.addPythonPoetryDependency(lambdas, api.runtime.python!);
 
 // Add commands to the lambda project's package task to create a distributable which can be deployed to AWS Lambda
 lambdas.packageTask.exec(`mkdir -p lambda-dist && rm -rf lambda-dist/*`);
-lambdas.packageTask.exec(`cp -r ${lambdas.moduleName} lambda-dist/${lambdas.moduleName}`);
-lambdas.packageTask.exec(`poetry export --without-hashes --format=requirements.txt > lambda-dist/requirements.txt`);
-lambdas.packageTask.exec(`pip install -r lambda-dist/requirements.txt --target lambda-dist --upgrade`);
-lambdas.gitignore.addPatterns('lambda-dist');
+lambdas.packageTask.exec(
+  `cp -r ${lambdas.moduleName} lambda-dist/${lambdas.moduleName}`
+);
+lambdas.packageTask.exec(
+  `poetry export --without-hashes --format=requirements.txt > lambda-dist/requirements.txt`
+);
+lambdas.packageTask.exec(
+  `pip install -r lambda-dist/requirements.txt --target lambda-dist --upgrade`
+);
+lambdas.gitignore.addPatterns("lambda-dist");
 
 // Create a CDK infrastructure project
 const infra = new AwsCdkPythonApp({
   name: "infra",
   parent: monorepo,
-  outdir: 'packages/infra',
+  outdir: "packages/infra",
   authorEmail: "me@example.com",
   authorName: "me",
   cdkVersion: "2.0.0",
   moduleName: "infra",
   version: "1.0.0",
   poetry: true,
 });
@@ -1343,31 +1414,31 @@
 import { NxMonorepoProject } from "@aws-prototyping-sdk/nx-monorepo";
 import { TypeSafeApiProject } from "@aws-prototyping-sdk/type-safe-api";
 import { AwsCdkTypeScriptApp } from "projen/lib/awscdk";
 import { JavaProject } from "projen/lib/java";
 
 // Create the monorepo
 const monorepo = new NxMonorepoProject({
-  name: 'monorepo',
+  name: "monorepo",
   defaultReleaseBranch: "main",
 });
 
 // Create the API project
 const api = new TypeSafeApiProject({
   name: "myapi",
   parent: monorepo,
-  outdir: 'packages/api',
+  outdir: "packages/api",
   // Smithy as the model language. You can also use ModelLanguage.OPENAPI
   model: {
     language: ModelLanguage.SMITHY,
     options: {
       smithy: {
         serviceName: {
-          namespace: 'com.mycompany',
-          serviceName: 'MyApi',
+          namespace: "com.mycompany",
+          serviceName: "MyApi",
         },
       },
     },
   },
   // Generate client and server types in TypeScript, Python and Java
   runtime: {
     languages: [Language.TYPESCRIPT, Language.PYTHON, Language.JAVA],
@@ -1381,15 +1452,15 @@
     formats: [DocumentationFormat.HTML_REDOC],
   },
 });
 
 const lambdas = new JavaProject({
   name: "lambdas",
   parent: monorepo,
-  outdir: 'packages/lambdas',
+  outdir: "packages/lambdas",
   artifactId: "lambdas",
   groupId: "com.my.api",
   version: "1.0.0",
 });
 
 // The lambdas package needs a dependency on the generated java runtime
 monorepo.addJavaDependency(lambdas, api.runtime.java!);
@@ -1407,15 +1478,15 @@
     },
   ],
 });
 
 const infra = new AwsCdkJavaApp({
   name: "infra",
   parent: monorepo,
-  outdir: 'packages/infra',
+  outdir: "packages/infra",
   artifactId: "infra",
   groupId: "com.my.api",
   mainClass: "com.my.api.MyApp",
   version: "1.0.0",
   cdkVersion: "2.0.0",
 });
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.5/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO` & `aws_prototyping_sdk.type_safe_api-0.18.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: aws-prototyping-sdk.type-safe-api
-Version: 0.18.5
-Summary: @aws-prototyping-sdk/type-safe-api
-Home-page: https://github.com/aws/aws-prototyping-sdk
-Author: AWS APJ COPE<apj-cope@amazon.com>
-License: Apache-2.0
-Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: JavaScript
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Typing :: Typed
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## Type Safe API
 
 Define your APIs using [Smithy](https://smithy.io/2.0/) or [OpenAPI v3](https://swagger.io/specification/), and leverage the power of generated client and server types, infrastructure, documentation, and automatic input validation!
 
 This package vends a projen project type which allows you to define an API using either [Smithy](https://smithy.io/2.0/) or [OpenAPI v3](https://swagger.io/specification/), and a construct which manages deploying this API in API Gateway, given an integration (eg a lambda) for every operation.
 
 The project will generate "runtime" projects from your API definition in your desired languages, which can be utilised both client side for interacting with your API, or server side for implementing your API. The project also generates a type-safe CDK construct which ensures an integration is provided for every API operation.
@@ -94,39 +70,41 @@
 ```
 
 #### Use the CDK Construct
 
 In your CDK application (ie within the `infra` project we created), consume the `Api` construct, vended from the generated typescript infrastructure package.
 
 ```python
-import { Stack, StackProps } from 'aws-cdk-lib';
-import { Construct } from 'constructs';
+import { Stack, StackProps } from "aws-cdk-lib";
+import { Construct } from "constructs";
 import { Api } from "myapi-typescript-infra"; // <- generated typescript infrastructure package
 import { Authorizers, Integrations } from "@aws-prototyping-sdk/type-safe-api";
 import { NodejsFunction } from "aws-cdk-lib/aws-lambda-nodejs";
 import { Cors } from "aws-cdk-lib/aws-apigateway";
-import * as path from 'path';
+import * as path from "path";
 
 export class MyStack extends Stack {
   constructor(scope: Construct, id: string, props: StackProps = {}) {
     super(scope, id, props);
 
     // Instantiate the generated CDK construct to deploy an API Gateway API based on your model
-    new Api(this, 'MyApi', {
+    new Api(this, "MyApi", {
       defaultAuthorizer: Authorizers.iam(),
       corsOptions: {
         allowOrigins: Cors.ALL_ORIGINS,
         allowMethods: Cors.ALL_METHODS,
       },
       // Supply an integration for every operation
       integrations: {
         sayHello: {
-          integration: Integrations.lambda(new NodejsFunction(this, 'SayHelloLambda', {
-            entry: path.resolve(__dirname, 'say-hello.ts'),
-          })),
+          integration: Integrations.lambda(
+            new NodejsFunction(this, "SayHelloLambda", {
+              entry: path.resolve(__dirname, "say-hello.ts"),
+            })
+          ),
         },
       },
     });
   }
 }
 ```
 
@@ -362,20 +340,20 @@
       parameters:
         - in: query
           name: name
           schema:
             type: string
           required: true
       responses:
-        '200':
+        "200":
           description: Successful response
           content:
-            'application/json':
+            "application/json":
               schema:
-                $ref: '#/components/schemas/HelloResponse'
+                $ref: "#/components/schemas/HelloResponse"
 components:
   schemas:
     HelloResponse:
       type: object
       properties:
         message:
           type: string
@@ -402,52 +380,52 @@
 
 ```yaml
 openapi: 3.0.3
 info:
   version: 1.0.0
   title: Example API
 paths:
-  $ref: './paths/index.yaml'
+  $ref: "./paths/index.yaml"
 components:
   schemas:
-    $ref: './schemas/index.yaml'
+    $ref: "./schemas/index.yaml"
 ```
 
 `paths/index.yaml`:
 
 ```yaml
 /hello:
   get:
-    $ref: './sayHello.yaml'
+    $ref: "./sayHello.yaml"
 ```
 
 `paths/sayHello.yaml`:
 
 ```yaml
 operationId: sayHello
 parameters:
- - in: query
-   name: name
-   schema:
-     type: string
-   required: true
+  - in: query
+    name: name
+    schema:
+      type: string
+    required: true
 responses:
-  '200':
+  "200":
     description: Successful response
     content:
-      'application/json':
+      "application/json":
         schema:
-          $ref: '../schemas/helloResponse.yaml'
+          $ref: "../schemas/helloResponse.yaml"
 ```
 
 `schemas/index.yaml`:
 
 ```yaml
 HelloResponse:
-  $ref: './helloResponse.yaml'
+  $ref: "./helloResponse.yaml"
 ```
 
 `schemas/helloResponse.yaml`:
 
 ```yaml
 type: object
 properties:
@@ -460,55 +438,57 @@
 ### Construct
 
 A CDK construct is generated in the `infrastructure/<language>` directory which provides a type-safe interface for creating an API Gateway API based on your model.
 
 You can extend or instantiate this construct in your CDK infrastructure project. You'll get a type error if you forget to define an integration for an operation defined in your api.
 
 ```python
-import { Authorizers, Integrations } from '@aws-prototyping-sdk/type-safe-api';
-import { NodejsFunction } from 'aws-cdk-lib/aws-lambda-nodejs';
-import { Construct } from 'constructs';
-import { Api } from 'myapi-typescript-infra';
+import { Authorizers, Integrations } from "@aws-prototyping-sdk/type-safe-api";
+import { NodejsFunction } from "aws-cdk-lib/aws-lambda-nodejs";
+import { Construct } from "constructs";
+import { Api } from "myapi-typescript-infra";
 
 /**
  * An example of how to wire lambda handler functions to the API
  */
 export class SampleApi extends Api {
   constructor(scope: Construct, id: string) {
     super(scope, id, {
       defaultAuthorizer: Authorizers.iam(),
       integrations: {
         // Every operation defined in your API must have an integration defined!
         sayHello: {
-          integration: Integrations.lambda(new NodejsFunction(scope, 'say-hello')),
+          integration: Integrations.lambda(
+            new NodejsFunction(scope, "say-hello")
+          ),
         },
       },
     });
   }
 }
 ```
 
 #### Sharing Integrations
 
 If you would like to use the same integration for every operation (for example you'd like to use a single lambda function to service all requests with the in-built [handler router](#handler-router)), you can use the `Operations.all` method from a generated runtime project to save repeating yourself:
 
 ```python
-import { Operations } from 'myapi-typescript-runtime';
-import { Authorizers, Integrations } from '@aws-prototyping-sdk/type-safe-api';
-import { NodejsFunction } from 'aws-cdk-lib/aws-lambda-nodejs';
-import { Construct } from 'constructs';
-import { Api } from 'myapi-typescript-infra';
+import { Operations } from "myapi-typescript-runtime";
+import { Authorizers, Integrations } from "@aws-prototyping-sdk/type-safe-api";
+import { NodejsFunction } from "aws-cdk-lib/aws-lambda-nodejs";
+import { Construct } from "constructs";
+import { Api } from "myapi-typescript-infra";
 
 export class SampleApi extends Api {
   constructor(scope: Construct, id: string) {
     super(scope, id, {
       defaultAuthorizer: Authorizers.iam(),
       // Use the same integration for every operation.
       integrations: Operations.all({
-        integration: Integrations.lambda(new NodejsFunction(scope, 'router')),
+        integration: Integrations.lambda(new NodejsFunction(scope, "router")),
       }),
     });
   }
 }
 ```
 
 TypeScript is demonstrated above, but this is also available in Java and Python.
@@ -526,29 +506,35 @@
 
 To use the Cognito authorizer, one or more user pools must be provided. You can optionally specify the scopes to check if using an access token. You can use the `withScopes` method to use the same authorizer but verify different scopes for individual integrations, for example:
 
 ```python
 export class SampleApi extends Api {
   constructor(scope: Construct, id: string) {
     const cognitoAuthorizer = Authorizers.cognito({
-      authorizerId: 'myCognitoAuthorizer',
-      userPools: [new UserPool(scope, 'UserPool')],
+      authorizerId: "myCognitoAuthorizer",
+      userPools: [new UserPool(scope, "UserPool")],
     });
 
     super(scope, id, {
       defaultAuthorizer: cognitoAuthorizer,
       integrations: {
         // Everyone in the user pool can call this operation:
         sayHello: {
-          integration: Integrations.lambda(new NodejsFunction(scope, 'say-hello')),
+          integration: Integrations.lambda(
+            new NodejsFunction(scope, "say-hello")
+          ),
         },
         // Only users with the given scopes can call this operation
         myRestrictedOperation: {
-          integration: Integrations.lambda(new NodejsFunction(scope, 'my-restricted-operation')),
-          authorizer: cognitoAuthorizer.withScopes('my-resource-server/my-scope'),
+          integration: Integrations.lambda(
+            new NodejsFunction(scope, "my-restricted-operation")
+          ),
+          authorizer: cognitoAuthorizer.withScopes(
+            "my-resource-server/my-scope"
+          ),
         },
       },
     });
   }
 }
 ```
 
@@ -558,27 +544,28 @@
 
 Custom authorizers use lambda functions to handle authorizing requests. These can either be simple token-based authorizers, or more complex request-based authorizers. See the [API Gateway documentation](https://docs.aws.amazon.com/apigateway/latest/developerguide/apigateway-use-lambda-authorizer.html) for more details.
 
 An example token-based authorizer (default):
 
 ```python
 Authorizers.custom({
-  authorizerId: 'myTokenAuthorizer',
-  function: new NodejsFunction(scope, 'authorizer'),
+  authorizerId: "myTokenAuthorizer",
+  function: new NodejsFunction(scope, "authorizer"),
 });
 ```
 
 An example request-based handler. By default the identitySource will be `method.request.header.Authorization`, however you can customise this as per [the API Gateway documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-apigateway-authorizer.html#cfn-apigateway-authorizer-identitysource).
 
 ```python
 Authorizers.custom({
-  authorizerId: 'myRequestAuthorizer',
+  authorizerId: "myRequestAuthorizer",
   type: CustomAuthorizerType.REQUEST,
-  identitySource: 'method.request.header.MyCustomHeader, method.request.querystring.myQueryString',
-  function: new NodejsFunction(scope, 'authorizer'),
+  identitySource:
+    "method.request.header.MyCustomHeader, method.request.querystring.myQueryString",
+  function: new NodejsFunction(scope, "authorizer"),
 });
 ```
 
 #### Integrations
 
 Integrations are used by API Gateway to service requests.
 
@@ -601,18 +588,20 @@
 The [typescript-fetch](https://openapi-generator.tech/docs/generators/typescript-fetch/) OpenAPI generator is used to generate typescript client. This requires an implementation of `fetch` to be passed to the client. In the browser one can pass the built in fetch, or in NodeJS you can use an implementation such as [node-fetch](https://www.npmjs.com/package/node-fetch).
 
 Example usage of the client in a website:
 
 ```python
 import { Configuration, DefaultApi } from "myapi-typescript-runtime";
 
-const client = new DefaultApi(new Configuration({
-  basePath: "https://xxxxxxxxxx.execute-api.ap-southeast-2.amazonaws.com",
-  fetchApi: window.fetch.bind(window),
-}));
+const client = new DefaultApi(
+  new Configuration({
+    basePath: "https://xxxxxxxxxx.execute-api.ap-southeast-2.amazonaws.com",
+    fetchApi: window.fetch.bind(window),
+  })
+);
 
 await client.sayHello({ name: "Jack" });
 ```
 
 #### Python
 
 The [python](https://openapi-generator.tech/docs/generators/python) OpenAPI generator is used to generate clients for python.
@@ -680,15 +669,19 @@
 ```
 
 ##### Handler Router
 
 The lambda handler wrappers can be used in isolation as handler methods for separate lambdas. If you would like to use a single lambda function to serve all requests, you can do so with the `handlerRouter`.
 
 ```python
-import { handlerRouter, sayHelloHandler, sayGoodbyeHandler } from "myapi-typescript-runtime";
+import {
+  handlerRouter,
+  sayHelloHandler,
+  sayGoodbyeHandler,
+} from "myapi-typescript-runtime";
 import { corsInterceptor } from "./interceptors";
 import { sayGoodbye } from "./handlers/say-goodbye";
 
 const sayHello = sayHelloHandler(async ({ input }) => {
   return {
     statusCode: 200,
     body: {
@@ -814,44 +807,65 @@
 import {
   sayHelloHandler,
   ChainedRequestInput,
   OperationResponse,
 } from "myapi-typescript-runtime";
 
 // Interceptor to wrap invocations in a try/catch, returning a 500 error for any unhandled exceptions.
-const tryCatchInterceptor = async <RequestParameters, RequestArrayParameters, RequestBody, Response>(
-  request: ChainedRequestInput<RequestParameters, RequestArrayParameters, RequestBody, Response>
+const tryCatchInterceptor = async <
+  RequestParameters,
+  RequestArrayParameters,
+  RequestBody,
+  Response
+>(
+  request: ChainedRequestInput<
+    RequestParameters,
+    RequestArrayParameters,
+    RequestBody,
+    Response
+  >
 ): Promise<Response | OperationResponse<500, { errorMessage: string }>> => {
   try {
     return await request.chain.next(request);
   } catch (e: any) {
-    return { statusCode: 500, body: { errorMessage: e.message }};
+    return { statusCode: 500, body: { errorMessage: e.message } };
   }
 };
 
 // tryCatchInterceptor is passed first, so it runs first and calls the second argument function (the request handler) via chain.next
-export const handler = sayHelloHandler(tryCatchInterceptor, async ({ input }) => {
-  return {
-    statusCode: 200,
-    body: {
-      message: `Hello ${input.requestParameters.name}!`,
-    },
-  };
-});
+export const handler = sayHelloHandler(
+  tryCatchInterceptor,
+  async ({ input }) => {
+    return {
+      statusCode: 200,
+      body: {
+        message: `Hello ${input.requestParameters.name}!`,
+      },
+    };
+  }
+);
 ```
 
 Another example interceptor might be to record request time metrics. The example below includes the full generic type signature for an interceptor:
 
 ```python
-import {
-  ChainedRequestInput,
-} from 'myapi-typescript-runtime';
+import { ChainedRequestInput } from "myapi-typescript-runtime";
 
-const timingInterceptor = async <RequestParameters, RequestArrayParameters, RequestBody, Response>(
-  request: ChainedRequestInput<RequestParameters, RequestArrayParameters, RequestBody, Response>
+const timingInterceptor = async <
+  RequestParameters,
+  RequestArrayParameters,
+  RequestBody,
+  Response
+>(
+  request: ChainedRequestInput<
+    RequestParameters,
+    RequestArrayParameters,
+    RequestBody,
+    Response
+  >
 ): Promise<Response> => {
   const start = Date.now();
   const response = await request.chain.next(request);
   const end = Date.now();
   console.log(`Took ${end - start} ms`);
   return response;
 };
@@ -859,18 +873,28 @@
 
 Interceptors may mutate the `interceptorContext` to pass state to further interceptors or the final lambda handler, for example an `identityInterceptor` might want to extract the authenticated user from the request so that it is available in handlers.
 
 ```python
 import {
   LambdaRequestParameters,
   LambdaHandlerChain,
-} from 'myapi-typescript-runtime';
+} from "myapi-typescript-runtime";
 
-const identityInterceptor = async <RequestParameters, RequestArrayParameters, RequestBody, Response>(
-  request: ChainedRequestInput<RequestParameters, RequestArrayParameters, RequestBody, Response>
+const identityInterceptor = async <
+  RequestParameters,
+  RequestArrayParameters,
+  RequestBody,
+  Response
+>(
+  request: ChainedRequestInput<
+    RequestParameters,
+    RequestArrayParameters,
+    RequestBody,
+    Response
+  >
 ): Promise<Response> => {
   const authenticatedUser = await getAuthenticatedUser(request.event);
   return await request.chain.next({
     ...request,
     interceptorContext: {
       ...request.interceptorContext,
       authenticatedUser,
@@ -1082,61 +1106,78 @@
 ```
 
 ##### Usage in a React Website
 
 First, make sure you create an instance of the API client (making sure to set the base URL and fetch instance). For example:
 
 ```python
-export const useMyApiClient = () => useMemo(() => new MyApi(new Configuration({
-  basePath: 'https://example123.execute-api.ap-southeast-2.amazonaws.com/prod',
-  fetchApi: window.fetch.bind(window),
-})), []);
+export const useMyApiClient = () =>
+  useMemo(
+    () =>
+      new MyApi(
+        new Configuration({
+          basePath:
+            "https://example123.execute-api.ap-southeast-2.amazonaws.com/prod",
+          fetchApi: window.fetch.bind(window),
+        })
+      ),
+    []
+  );
 ```
 
 Note that if you are using the [Cloudscape React Website](../cloudscape-react-ts-website/README.md) with [AWS NorthStar](https://aws.github.io/aws-northstar/) and IAM (Sigv4) Auth for your API, you can use NorthStar's [`useSigv4Client()` hook](https://aws.github.io/aws-northstar/?path=/story/components-cognitoauth-sigv4client-docs--page) to create
 an instance of `fetch` which will sign requests with the logged in user's credentials. For example:
 
 ```python
 export const useMyApiClient = () => {
-  const { client } = useSigv4Client();
-  return useMemo(() => client.current ? new MyApi(new Configuration({
-    basePath: 'https://example123.execute-api.ap-southeast-2.amazonaws.com/prod',
-    fetchApi: client.current,
-  })) : undefined, [client.current]);
+  const client = useSigv4Client();
+  return useMemo(
+    () =>
+      client
+        ? new MyApi(
+            new Configuration({
+              basePath:
+                "https://example123.execute-api.ap-southeast-2.amazonaws.com/prod",
+              fetchApi: client,
+            })
+          )
+        : undefined,
+    [client]
+  );
 };
 ```
 
 Next, instantiate the client provider above where you would like to use the hooks in your component hierarchy (such as above your router). For example:
 
 ```tsx
+import { DefaultApiClientProvider } from "myapi-typescript-react-query-hooks";
+
 const api = useMyApiClient();
 
 return api ? (
-  <MyApiClientContext.Provider value={api}>
-    { /* Components within the provider may make use of the hooks */ }
-  </MyApiClientContext.Provider>
-) : <p>Loading...</p>;
+  <DefaultApiClientProvider apiClient={api}>
+    {/* Components within the provider may make use of the hooks */}
+  </DefaultApiClientProvider>
+) : (
+  <p>Loading...</p>
+);
 ```
 
 Finally, you can import and use your generated hooks. For example:
 
 ```tsx
 export const MyComponent: FC<MyComponentProps> = () => {
-  const sayHello = useSayHello({ name: 'World' });
+  const sayHello = useSayHello({ name: "World" });
 
-  return (
-    sayHello.isLoading ? (
-      <p>Loading...</p>
-    ) : (
-      sayHello.isError ? (
-        <p>Error!</p>
-      ) : (
-        <h1>{sayHello.data.message}</h1>
-      )
-    )
+  return sayHello.isLoading ? (
+    <p>Loading...</p>
+  ) : sayHello.isError ? (
+    <p>Error!</p>
+  ) : (
+    <h1>{sayHello.data.message}</h1>
   );
 };
 ```
 
 ##### Paginated Operations
 
 You can generate `useInfiniteQuery` hooks instead of `useQuery` hooks for paginated API operations, by making use of the vendor extension `x-paginated` in your operation in the OpenAPI specification. You must specify both the `inputToken` and `outputToken`, which indicate the properties from the input and output used for pagination. For example in OpenAPI:
@@ -1216,77 +1257,83 @@
 import { NxMonorepoProject } from "@aws-prototyping-sdk/nx-monorepo";
 import { TypeSafeApiProject } from "@aws-prototyping-sdk/type-safe-api";
 import { AwsCdkTypeScriptApp } from "projen/lib/awscdk";
 import { PythonProject } from "projen/lib/python";
 
 // Create the monorepo
 const monorepo = new NxMonorepoProject({
-  name: 'monorepo',
+  name: "monorepo",
   defaultReleaseBranch: "main",
 });
 
 // Create the API project
 const api = new TypeSafeApiProject({
   name: "myapi",
   parent: monorepo,
-  outdir: 'packages/api',
+  outdir: "packages/api",
   // Smithy as the model language. You can also use ModelLanguage.OPENAPI
   model: {
     language: ModelLanguage.SMITHY,
     options: {
       smithy: {
         serviceName: {
-          namespace: 'com.mycompany',
-          serviceName: 'MyApi',
+          namespace: "com.mycompany",
+          serviceName: "MyApi",
         },
       },
     },
   },
   // Generate client and server types in TypeScript, Python, and Java
   runtime: {
     languages: [Language.TYPESCRIPT, Language.PYTHON, Language.JAVA],
   },
   // Generate CDK infrastructure in Python
   infrastructure: {
     language: Language.PYTHON,
   },
   // Generate HTML documentation
   documentation: {
-    formats: [DocumentationFormat.HTML_REDOC]
+    formats: [DocumentationFormat.HTML_REDOC],
   },
 });
 
 // Create a project for our lambda handlers written in python
 const lambdas = new PythonProject({
   name: "lambdas",
   parent: monorepo,
-  outdir: 'packages/lambdas',
+  outdir: "packages/lambdas",
   authorEmail: "me@example.com",
   authorName: "me",
   moduleName: "lambdas",
   version: "1.0.0",
   // Poetry is used to simplify local python dependencies
   poetry: true,
 });
 
 // Add a local dependency on the generated python runtime
 monorepo.addPythonPoetryDependency(lambdas, api.runtime.python!);
 
 // Add commands to the lambda project's package task to create a distributable which can be deployed to AWS Lambda
 lambdas.packageTask.exec(`mkdir -p lambda-dist && rm -rf lambda-dist/*`);
-lambdas.packageTask.exec(`cp -r ${lambdas.moduleName} lambda-dist/${lambdas.moduleName}`);
-lambdas.packageTask.exec(`poetry export --without-hashes --format=requirements.txt > lambda-dist/requirements.txt`);
-lambdas.packageTask.exec(`pip install -r lambda-dist/requirements.txt --target lambda-dist --upgrade`);
-lambdas.gitignore.addPatterns('lambda-dist');
+lambdas.packageTask.exec(
+  `cp -r ${lambdas.moduleName} lambda-dist/${lambdas.moduleName}`
+);
+lambdas.packageTask.exec(
+  `poetry export --without-hashes --format=requirements.txt > lambda-dist/requirements.txt`
+);
+lambdas.packageTask.exec(
+  `pip install -r lambda-dist/requirements.txt --target lambda-dist --upgrade`
+);
+lambdas.gitignore.addPatterns("lambda-dist");
 
 // Create a CDK infrastructure project
 const infra = new AwsCdkPythonApp({
   name: "infra",
   parent: monorepo,
-  outdir: 'packages/infra',
+  outdir: "packages/infra",
   authorEmail: "me@example.com",
   authorName: "me",
   cdkVersion: "2.0.0",
   moduleName: "infra",
   version: "1.0.0",
   poetry: true,
 });
@@ -1366,31 +1413,31 @@
 import { NxMonorepoProject } from "@aws-prototyping-sdk/nx-monorepo";
 import { TypeSafeApiProject } from "@aws-prototyping-sdk/type-safe-api";
 import { AwsCdkTypeScriptApp } from "projen/lib/awscdk";
 import { JavaProject } from "projen/lib/java";
 
 // Create the monorepo
 const monorepo = new NxMonorepoProject({
-  name: 'monorepo',
+  name: "monorepo",
   defaultReleaseBranch: "main",
 });
 
 // Create the API project
 const api = new TypeSafeApiProject({
   name: "myapi",
   parent: monorepo,
-  outdir: 'packages/api',
+  outdir: "packages/api",
   // Smithy as the model language. You can also use ModelLanguage.OPENAPI
   model: {
     language: ModelLanguage.SMITHY,
     options: {
       smithy: {
         serviceName: {
-          namespace: 'com.mycompany',
-          serviceName: 'MyApi',
+          namespace: "com.mycompany",
+          serviceName: "MyApi",
         },
       },
     },
   },
   // Generate client and server types in TypeScript, Python and Java
   runtime: {
     languages: [Language.TYPESCRIPT, Language.PYTHON, Language.JAVA],
@@ -1404,15 +1451,15 @@
     formats: [DocumentationFormat.HTML_REDOC],
   },
 });
 
 const lambdas = new JavaProject({
   name: "lambdas",
   parent: monorepo,
-  outdir: 'packages/lambdas',
+  outdir: "packages/lambdas",
   artifactId: "lambdas",
   groupId: "com.my.api",
   version: "1.0.0",
 });
 
 // The lambdas package needs a dependency on the generated java runtime
 monorepo.addJavaDependency(lambdas, api.runtime.java!);
@@ -1430,15 +1477,15 @@
     },
   ],
 });
 
 const infra = new AwsCdkJavaApp({
   name: "infra",
   parent: monorepo,
-  outdir: 'packages/infra',
+  outdir: "packages/infra",
   artifactId: "infra",
   groupId: "com.my.api",
   mainClass: "com.my.api.MyApp",
   version: "1.0.0",
   cdkVersion: "2.0.0",
 });
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.5/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt` & `aws_prototyping_sdk.type_safe_api-0.18.6/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
 src/aws_prototyping_sdk/type_safe_api/__init__.py
 src/aws_prototyping_sdk/type_safe_api/py.typed
 src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
-src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.18.5.jsii.tgz
+src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.18.6.jsii.tgz
```

