# Custom Toggled Elements

Toggled supports a variety of custom HTML blocks to make your life easier.

## Email Signup

Create a mailing list signup which will display on your dashboard.

```html
<toggledEmail data-name="<nickname>"></toggledEmail>
```

You can have multiple of these on each page.

Nickname will be displayed on your dashboard so you can see which forms are converting users to subscribers.

### DEMO
<toggledEmail data-name="DEMO"></toggledEmail>

## Analytics

Use Google Analytics in your project.

```html
<googleAnalytics data-tag="<YOUR ANALYTICS MEASUREMENT ID>"></googleAnalytics>
```

Only one element per page is supported.

Keep in mind that Toggled will soon have built-in analytics.

## Toggled Designs

To import designs from external websites such as Codepen, Spline Etc. in Toggled, you must use the design manager. (If you try to use the js libraries from these providers they will not work in Toggled to prevent xss)

Below is an example for Spline.

```html
<design data-layout="3D" data-type="spline" data-url="https://prod.spline.design/Iu9kNCw-o9kUZfGj/scene.splinecode"></design>
```

Below is an example for Codepen. (Please use the special embed link provided.)

```html
<design data-layout="2D" data-type="codepen" data-url="https://codepen.io/lavadev/embed/MWzxaQR?default-tab=html%2Cresult"></design>
```

Below is an example for Replit. (Please just use your Replit Project url not the embed URL)

```html
<design data-layout="2D" data-type="replit" data-url="https://replit.com/@CosmixCom/GravityAI"></design>
```

Below is an example for Scratch. (Please just use your Project ID)

```html
<design data-layout="2D" data-type="scratch" data-projectID="923122579"></design>
```

data-layout: 3D or 2D <br>
data-type: Type of design. (E.g. Spline) * <br>
data-url: CND/Embed URL of design * <br>

### Toggled Status

Ping pages to check the status.

There are two outputs ONLINE or OFFLINE. Toggled sends a GET request to the specified URL. (Include https)

```html
<toggledStatus data-url="<URL TO PING>"></toggledStatus>
```

If this page returns 404, 403, 500 etc. it will return offline. The page must return an `"ok"` request to be online.
