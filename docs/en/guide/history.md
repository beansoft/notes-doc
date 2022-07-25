---
title: History changes
icon: changelog
---

::: danger Announcement
**2022.1.4** starts to charge,Please refer to the purchase **License** process in [**Buy plugin**](./buy.md)

Click to join **Telegram Group**↓↓↓

[![Telegram](https://img.shields.io/static/v1?label=Telegram&message=Restful%20Fast%20Request&logo=telegram&color=32CD32)](https://t.me/restful_fast_request)

Issue please goto [Github](https://github.com/dromara/fast-request/issues)

:::

## v2022.2.1<Badge text="Charge" type="warn"/><Badge text="Newest version" type="tip"/>
* API grouping parameter save support
* Temporary request save support
* Add support for cURL import
* Add Response Header in response
* Add support for Url suffix
* Optimized parameter parsing
* Fix Word export bug
* Optimize shortcut keys

::: tip API grouping parameter save support
Purpose: Save parameters of different combinations under one API

==The original save operation will be classified into the Default group by default==

![groupSave](../../.vuepress/public/img/2022.2.1/groupSave_en.png)

**Toggle parameter**

The following is the query of the book list in 3 languages

![apiParamGroup](../../.vuepress/public/img/2022.2.1/apiParamGroup_en.gif)
:::

::: info Temporary request save support

Purpose: Save any request that does not belong to this project for temporary invocation, not associated with the current project code

The Url of the Request saved by the temporary request must start with ==http== or ==https==

![tempSave](../../.vuepress/public/img/2022.2.1/tempSave_en.png)

:::

::: tip cURL import

![importByCurl](../../.vuepress/public/img/2022.2.1/importByCurl_en.gif)

==Note that if you need to bind a method, you need to place the cursor on the method name==
:::


::: info Add Response Header in response

![responseHeader](../../.vuepress/public/img/2022.2.1/responseHeader.png)

:::

::: info Add support for Url suffix

Purpose: Some requests need to add .do at the end of the url

![responseHeader](../../.vuepress/public/img/2022.2.1/urlSuffix.png)

:::

::: note Optimized parameter parsing
Optimized parsing of `List<Entity>`
:::

## v2022.1.10<Badge text="Charge" type="warn"/>
* Add support for history request preview
* Add support for description search in SearchEveryWhere
* Shortcut key conflict optimization
* Add request timeout settings
* Text editor character display cursor positioning optimization
* Curl output format optimization
* Optimization @Consumes(APPLICATION_JSON) ineffective problem(JAX-RS)

::: tip Add support for history request preview
Hidden skills: Double-click the record to display details
![history](../../.vuepress/public/img/history.png)
:::

::: info Add support for description search in SearchEveryWhere
Support description search API
![searchEveryWhereDescription](../../.vuepress/public/img/searchEveryWhereDescription.png)
:::


::: danger Add request timeout settings
Default value: 60 seconds
![timeoutSetting](../../.vuepress/public/img/timeoutSetting.png)
:::


::: note Optimization
* Shortcut key conflict optimization
  * Added Shift to the three shortcut keys for opening windows
* Text editor character display cursor positioning optimization
  * When the text editor generates a string, it focuses on the first line by default
:::

## v2022.1.9<Badge text="Charge" type="warn"/>
* Add shortcut keys for tool window jump
* Ignore field parsing optimizations
* Generic parameter parsing support
* Improve project global config
* Add auto add cookie support
* Fixed bug when editing params at the same time delete param
* Interface optimization
* Save API insertion order optimization
* Add support for html preview in response raw
* APIs list view optimization
* Optimized export preview


::: tip Add shortcut keys for tool window jump
Provides shortcut keys to jump quickly, you can change it in `setting -> Keymap`
![toolwindowShortcut](../../.vuepress/public/img/toolwindowShortcut.png)
:::

::: info Ignore field parsing optimizations
* Ignore parsing annotated by `@JsonIgnore`、`@JSONField(serialize = false)` fields
* Ignore parsing`transient` keyword-decorated fields
  :::

::: info Generic parameter parsing support
Support for such generic parameter parsing
```java
@Data
public class CommonDTO<T,R> implements Serializable {
    private String accessToken;
    private String appKey;
    private String clientId;
    private T data;
    private List<R> dataList;
}

@PostMapping(value = "/apply")
public Integer loanApply(@RequestBody CommonDTO<Book, TestDTO> req){
    return 1;
}
```
:::

::: danger Improve project global config
Added `URL Params`、`URL-Encoded Params`、`Cookies`
![projectConfigParam](../../.vuepress/public/img/projectGlobalParam.png)
:::


::: tip Add auto add cookie support
Then automatically stored in == project global parameters ==
If enable this configuration,cookie will automatically store in ==Project Global Config== -> `cookies`,This configuration is enabled by default.
![autoStoreCookie](../../.vuepress/public/img/autoStoreCookie.png)
:::

::: note Optimization
* Interface optimization
  * Optimized tab spacing(narrow under windows)、background color
* Save API insertion order optimization
  * The post-saved API will be placed on top
:::

::: info Add support for html preview in response raw
The response of the html return type is no longer truncated in raw, and the html can be previewed at the same time

![rawHtmlPreview](../../.vuepress/public/img/rawHtmlPreview.png)
:::

::: tip APIs list view optimization
The rendering of the APIs interface has been optimized,Newly saved api icons are automatically optimized by default,The API saved in history can be right-clicked to select and change
![apisList](../../.vuepress/public/img/apisList.png)
:::

## v2022.1.8<Badge text="Charge" type="warn"/>
* Project-level global parameters support
* Optimized response data quickly add to headers
* Optimized cookies quickly added to the header
* Postman export optimization
* Fix navigate tree scan bug
* fix some bug

::: tip Project-level global parameters support

Support global parameters within the project level, not affected by multiple modules.

Configure priority `api header > project header>global header`

![projectConfigParam](../../.vuepress/public/img/projectConfigParam.png)
:::

::: info Quickly add to header parameters

Change ~~add params to global header~~ to `add params to project global header` 

Cookie is also like this

![add2projectConfig](../../.vuepress/public/img/add2projectConfig.png)

![cookie2projectConfig](../../.vuepress/public/img/cookie2projectConfig.png)
:::

## v2022.1.7<Badge text="Charge" type="warn"/>
* Kotlin spring framework support
* Add SearchEveryWhere scope search strategy
* Add toggleUseSoftWrap support in editor
* Add support for add to Global Header from response
* Optimize automatic binding projectName for saved api under multiple modules
* Add support for navigating to the current method

::: tip Kotlin spring framework support
![kotlinSupport](../../.vuepress/public/img/kotlinSupport.png)
:::

::: info Add SearchEveryWhere scope search strategy
The 2022.1.7 version can search for mapping in SpringBoot feign or controller by default

The default search strategy is to search based on annotations, and two options are provided. If you need to exclude interfaces similar in SpringBoot feign interface during the search process, you can remove the check of Interface to deal with it.
![searchEveryWhereStrategy](../../.vuepress/public/img/searchEveryWhereStrategy.png)
:::

::: note Add toggleUseSoftWrap support in editor

![toggleUseSoftWrap](../../.vuepress/public/img/toggleUseSoftWrap.png)
:::

::: tip Add support for add to Global Header from response
It is recommended to use in multi-module projects, because Add to Headers can only be added to the current module project

![add2GlobalHeader](../../.vuepress/public/img/add2GlobalHeader.png)
:::

::: info Optimize automatic binding projectName for saved api under multiple modules
Optimized the need to manually switch the project drop-down box for the saved api echo under the multi-module
:::

::: note Add support for navigating to the current method
After you generate the url of the method, sometimes you will switch to another place in the code, and then want to start debugging the API method, you can use this function to quickly locate the code

![navigate2CurrentMethod](../../.vuepress/public/img/navigate2CurrentMethod.png)
:::

## v2022.1.6<Badge text="Charge" type="warn"/>
* Add support for one click to add cookie to header
* Add support for sharing API to Word and html
* Fix bug for `Basic Authorization` don't carry Basic
* Add YouTrack bug support
* Removes the drag function in APIs tab

::: tip Add support for one click to add cookie to header

For those that require cookie support for login, you can quickly add the cookie in the response to the Header to achieve this

![addCookie2Header](../../.vuepress/public/img/addCookie2Header.png)
:::

::: info Add support for sharing API to Word and html

Please note that the API in word form is implemented in html, so don't feel strange, just export it

![shareApi](../../.vuepress/public/img/shareApi_en.png)
:::

::: note Add YouTrack bug support

Fast Request has enabled the automatic reporting bug to YouTrack. Just one click,No need to manually copy and paste it to Github to report bugs

Fast Request YouTrack website: [https://darkings.youtrack.cloud/issues](https://darkings.youtrack.cloud/issues)

![youtrackSubmit](../../.vuepress/public/img/youtrackSubmit.png)
:::


## v2022.1.5 <Badge text="Charge" type="warn"/>
* Remove text/html in Accept param in default header
* Add support for automatically generating parameter descriptions
* Add support for generate API documentation
* Add support for single class API list preview
* Fix some bugs

::: tip Add support for automatically generating parameter descriptions

You can hide or show description by toggle click

![paramDescription](../../.vuepress/public/img/paramDescription.png)
:::

::: info Add support for generate API documentation

After generating parameters, you can generate a Markdown document directly by sharing

![shareDocButton](../../.vuepress/public/img/shareDocButton.png)

![apiDocExample](../../.vuepress/public/img/apiDocExample.png)

:::

::: note Add support for single class API list preview

After focusing on the window, enter the keyword, and you can quickly search according to the path keyword of the API

![apiDocExample](../../.vuepress/public/img/apiPreview.gif)
:::


## v2022.1.4 <Badge text="Charge" type="warn"/>
==require idea 2021.3+==
* SearchEveryWhere highlight optimization
* Add support for import and export APIs
* Add support for run APIs
* Add timeout for api request
* Compatible with idea 2022.1
* Make it optional for automatically generate parameters
* Swagger annotation default value parameter parsing support
* Merged Send and Send and Download buttons
* APIs user interface optimization
* API Navigate rename to Navigate in tab
* Optimize the user guide of features
* Url generation optimization
* Fix Light files should have PSI only in one project

::: info SearchEveryWhere highlight optimization
Highlight search keywords to speed up the search for the API you really want to find.At the same time, the javadoc corresponding to the api is displayed

![help](../../.vuepress/public/img/searchEveryWhereHighlight.png)
:::

::: tip Add support for import and export APIs
Using this function, you can easily share your existing APIs with other developers, or import to IDEA on other devices
![exportImportApis](../../.vuepress/public/img/exportImportApis.gif)

More info **[Features->APIs import and export](./feature.md#apis-import-and-export)**
:::

::: warning Add support for run APIs
You can run your saved requests directly in the APIs tab

![runInApiManagement](../../.vuepress/public/img/runInApiManagement.png)
:::


:::note Automatically generate parameter optionals
![generateSwitch](../../.vuepress/public/img/generateSwitch_en.png)
:::

:::info Merged Send and Send and Download buttons
The buttons have been merged, because we usually use Send but not Send and Download, which reduces the number of toolbar buttons and looks simpler
![mergeRunAndDownload](../../.vuepress/public/img/mergeRunAndDownload.png)
:::

::: danger Swagger default value parsing support
Added the parsing of the default value of swagger annotations, which is more user-friendly of input parameters
* @ApiParam(swagger2)
* @ApiImplicitParam(swagger2)
* @ApiModelProperty(swagger2)
* @Parameter(swagger3)
* @Schema(swagger3)

More info **[Features->swagger default value parsing support](./feature.md#swagger-default-value-parsing-support)**
:::

::: tip Optimize the user guide of features
We have added a ? option in different windows to display some guidelines. For first-time users, it's easier to operate

And with the iteration of the version, more prompt operation guidelines may be added in the future

![help](../../.vuepress/public/img/help.png)
:::

::: info Url generation optimization
Historical logic will only take the first url, that is, test1, considering that in actual use, it is possible that you need another url, so random support has been added.

The following method url will be randomly generated to **/url1/test1,/url1/test2,/url2/test1,/url2/test2** by click <i class="icon iconfont icon-restfulFastRequest"></i>
```java
@RequestMapping({"url1","url2"})
@RestController
public class MultiUrlController {
    @GetMapping(value = {"test1","test2"})
    public Integer testUrl(){
        return 1;
    }
}
```

Expression support. The following demo url will be generated to **/url/public/test1**
```java
public class Constant {
  public static final String PUBLIC_URL = "/public";
}
@RequestMapping("url")
@RestController
public class MultiUrlController {
  @GetMapping(value = Constant.PUBLIC_URL + "/test1")
  public Integer testUrl(){
    return 1;
  }
}
```
:::

::: note API Navigate rename to Navigate in tab  
In the case where the tool window is relatively small, the API Navigate will be hidden. In order to display more content in the smallest tool window as possible, the name is shorter.
:::

## v2.1.3
* Add encode support for special symbol in parameter
* Add global headers to curl

## v2.1.2

* Add support for export api to Postman
* Open the idea lazy loading API Navigate tree for the first time
* SearchEveryWhere show module
* Optimize URL parsing
* Optimize the display of api navigate tree
* Optimize the group when save api
* Global header params support


:::tip Optimize URL parsing
support parse like following example

no longer need to configure the URL Replace Config separately
:::


:::: code-group

::: code-group-item Scene 1: URLS are class constant references

```java
@RequestMapping(Url1.URL_TEST)
@RestController
public class UrlTestController {
    private static final String URL= "xxx";

    @GetMapping(value = URL)
    public Integer testUrl(){
        return 1;
    }
}
```

:::

::: code-group-item Scene 2: value is an array

```java
@RequestMapping(
    value = {"/v1/save"},
    method = {RequestMethod.POST}
)
```

:::

::::


:::tip Add support for export api to Postman

![export2postman](../../.vuepress/public/img/export2postman.gif)
:::

:::tip SearchEveryWhere show module

![searchEveryWhereModule](../../.vuepress/public/img/searchEveryWhereModule.png)
:::

:::tip Optimize the group when save api

```
when saving the api,it will save to a group named controller's name

```

![save2ControllerGroup](../../.vuepress/public/img/save2ControllerGroup.png)
:::

:::tip Global header params support

![globalRequestHeader](../../.vuepress/public/img/globalRequestHeader.png)
:::

## v2.1.1

* SearchEveryWhere support
* Add a what's new button to view the latest version at any time
* Optimize the parsing of enum
* Add support for http redirect

:::tip SearchEveryWhere support

```
example
/url  
get /list         (used for search get method)
post /save        (used for search post method)
```

![searchEveryWhere](../../.vuepress/public/img/searchEveryWhere.gif)
:::

:::tip Quick view of the latest version
![whatsnewNotifcation](../../.vuepress/public/img/whatsnewNotifcation.png)
:::

## v2.1.0.2

* Joined the organization [**Dromara**](https://dromara.org/zh/)(An organization dedicated to native solutions for the
  microservice cloud)

## v2.1.0.1

* Fix get param error

## v2.1.0

* Fix post api parse error when using @RequestBody and @RequestParam
* Parsing support for nested classes
* Add support for url parse from the path property of the @RequestMapping in controller class level
* Added support for Api Tree scanning with @RequestMapping class

## v2.0.9

* Fix "Slow operations are prohibited on EDT" for 2021.3+
* Fix add headers from response
* Add project-level configuration,env and project will not change while switch project
* Add format action icon to textEditor

:::tip Add headers from response

```
if your api need token in header,you can do like this to add params to header from response
```

![format](../../.vuepress/public/img/quickAddHeaders.gif)
:::

:::tip Add format action icon to textEditor
![format](../../.vuepress/public/img/format.gif)
:::

## v2.0.8.1

* Fix conflicting error when searchEveryWhere
* Adjust position of toolbar action button
* remove unnecessary dependence,size 11.1M->5.9M

## v2.0.8

* Fix npe when first add project/env
* Json tree response character rendering maximum limit
* Add support for filter by methodType in Api navigate
* Add support for ignoring parameter parsing
* Fix some EDT problem
* Send/sendDownload button support for custom shortcut keys
* Fix response text not show in 2021.3

:::tip send/sendDownload button support for custom shortcut keys

```
shortcut is available anywhere to trigger the event,No longer need to focus on the tool window
```

![shortcutSendAndDownload](../../.vuepress/public/img/shortcutSendAndDownload.png)
:::

:::tip Add support for filter by methodType in Api navigate
![shortcutSendAndDownload](../../.vuepress/public/img/methodFilter.png)
:::

## v2.0.7

* Add support for api navigate tree
* Add support for automatic switching of Headers with project and environment switching
* Optimized Windows system. In some cases, downloading files cannot pop up the directory
* Optimize the parameter parse of @RequestParam
* Optimize tool window project and env drop-down components and layout
* Optimize the prompt message of curl copy
* Optimize the prompt message of curl regenerate
* Add confirm operation when delete project and env config
* Fix the order of json field output is disrupted
* Move send button to toolbar and support keyboard shortcut

:::tip API navigate tree
```
Select the tree and enter keywords
Press Enter again or double-click the left mouse button to locate the API

Hover the mouse to display the doc of the api
```

![apinavi](../../.vuepress/public/img/apinav.gif)
:::

:::tip Headers Automatic switching
```
Scenes:Multi-module projects such as SpringBoot have different header parameters in different projects and different environments. 
In order to quickly switch headers, header grouping is coming.  
Operation method：
1.Modify in the headers group, constraint: the input value must be in standard json format
2.Switch the environment or project name directly, and then enter the corresponding key and value values in the headers form
```

![headerSwitch](../../.vuepress/public/img/headerSwitch.gif)
:::

:::tip Optimize the parameter parse of @RequestParam
@RequestParam parameters will be prioritized according to the alias  
`@RequestParam("nameAlias")List<String> nameList` param name will be nameAlias
:::


:::tip Move send button to toolbar and support keyboard shortcut
```
send request: alt =
send and download: alt -  
Prerequisites:Tool window needs to be focused
```

![toolbarSend](../../.vuepress/public/img/toolbarSend.png)
:::

:::tip Optimize tool window project and env drop-down box and layout
```
Icon p represents project
Icon e represents environment  
```

![dropdownProject](../../.vuepress/public/img/dropdownProject.png)

![dropdownEnv](../../.vuepress/public/img/dropdownEnv.png)
:::


## v2.0.6
* Fix "Light files should have PSI only in one project"
* Add support for json syntax check
* Add support for PATCH method
* Added support for saving the API to the corresponding module group
* Fix null value in response not output
* Add support for JAX-RS
* Display what's new

Without affecting the use, sometimes it will pop up "*Light files should have PSI only in one project"*.This has fixed in 2.0.6

::: tip json grammar check
![json](../../.vuepress/public/img/json_en.png)
:::

::: tip API group automatic association
![apiGroup](../../.vuepress/public/img/apiGroup_en.gif)

Module supports quick search
![apiGroup](../../.vuepress/public/img/moduleSearch.gif)
:::

::: tip JAX-RS support
![apiGroup](../../.vuepress/public/img/jaxrs.gif)
:::

::: tip Show what's new  
Will only be shown once
![apiGroup](../../.vuepress/public/img/whatsnew_en.png)
:::

## v2.0.5

* JSON built-in editor support
* Fix checkbox hidden when change param by text
* Fix headers param show error when reshow the api
* Optimized the request progress bar display

## v2.0.4

* Fix the interface confusion caused by the response content aisle
* Optimization of response JSON ultra long display
* Optimized icon size
* Migrate Chinese documents to Gitee

## v2.0.3

*   Add confirmation when deleting api
*   Added the support of selecting all parameters and inverting selection
*   Fix param parse for java.util.Set
*   Fix parse like 【@RequestParam
*   Fix the confusion of the quick add header interface

## v2.0.2

*   Fix that the A request is displayed to the B project in the case of multiple open projects
*   Fix array and list param parse error decorate by @ResponseBody
*   Fix List without generic parse error
*   Add support for send and download
*   Show progressbar while sending request
*   Brand new document\[click the doc icon in the toolbar\]
*   Some optimization

## v2.0.1

*   rename from Fast Request to Restful Fast Request
*   merge Json、Form URL-Encoded、Multipart to Body Tab to reduce the tool window width
*   fix bug when modify config in global mode
*   add get、post、delete、put icon to saved request
*   saved request support more search strategy
*   rename tab name from collection to APIs
*   support parse java.time.YearMonth

## v2.0.0

*   support store request
*   support params optional
*   optimal iu
*   fix some bugs