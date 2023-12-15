# Custom Toggled Elements

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

Below is an example for Codepen.

```html
<design data-layout="2D" data-type="codepen" data-url="https://codepen.io/lavadev/embed/MWzxaQR?default-tab=html%2Cresult"></design>
```

Below is an example for Replit.

```html
<design data-layout="2D" data-type="replit" data-url="https://replit.com/@CosmixCom/GravityAI"></design>
```

data-layout: 3D or 2D <br>
data-type: Type of design. (E.g. Spline) * <br>
data-url: CND/Embed URL of design * <br>

