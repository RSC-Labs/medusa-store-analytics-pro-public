# Medusa Store Analytics Pro

## What is it?

Medusa Store Analytics Pro is the extended version of very popular plugin - [Store Analytics](https://github.com/RSC-Labs/medusa-store-analytics).

This repository has been created for instruction purposes and as a place for raising bugs and improvements.

It is a commercial software so it requires a licence to be used.

## Found a bug or looking for an improvement?

Please raise an issue in Github issues.

## Installation

1. Install plugin by adding to your `package.json`:

```json
...
"@rsc-labs/medusa-store-analytics-pro-v2": "1.1.1" // or other available version
...
```
and execute install, e.g. `yarn install`.

2. Add plugin to your `medusa-config.js` with the licence key, which you received:

```js
...
plugins: [
    {
      resolve: "@rsc-labs/medusa-store-analytics-pro-v2",
      options: {
        licenceKey: <licence-key>
      }
    }
]
...
```

### Configuration

Plugin supports one additional option which you can pass into `options`. It is related to statistic `Abandoned average value`, which tells that customers did not finalize the cart. By default, abandoned cart is the one which was not updated in the last 7 days. You can configure it by your own. For instance, if cart needs to be treat as abandoned because it was not updated 20 days ago, then your configuration will look like this:
```js
...
plugins: [
    {
      resolve: "@rsc-labs/medusa-store-analytics-pro-v2",
      options: {
        licenceKey: <licence-key>,
        abandonedCartTimeInDays: 20
      }
    }
]
...
```

## Available functionalities

<ul>
  <li>Highly customizable dashboard, where you can choose any statistics you would like to see <span class="text-green-600 font-semibold">(PRO)</span></li>
  <li>Calendars for choosing date ranges <span class="text-green-600 font-semibold">(PRO)</span></li>
  <li>Choosing currency code just one time for all statistics <span class="text-green-600 font-semibold">(PRO)</span></li>
  <li>Filtering by orders' status <span class="text-green-600 font-semibold">(PRO)</span></li>
  <li>Advanced report in PDF with various statistics <span class="text-green-600 font-semibold">(PRO)</span></li>
</ul>

<h2 class="mt-6 text-lg font-semibold">Supported Statistics</h2>

<h3 class="mt-4 text-md font-semibold">Cart</h3>
<ul>
  <li>Breakdown for cart progress <span class="text-green-600 font-semibold">(PRO)</span></li>
  <li>Average value of cart <span class="text-green-600 font-semibold">(PRO)</span></li>
  <li>Abandoned average value <span class="text-green-600 font-semibold">(PRO)</span></li>
</ul>

<h3 class="mt-4 text-md font-semibold">Orders</h3>
<ul>
  <li>Refunds to orders <span class="text-green-600 font-semibold">(PRO)</span></li>
  <li>Promotions to orders <span class="text-green-600 font-semibold">(PRO)</span></li>
  <li>Total promotions from orders <span class="text-green-600 font-semibold">(PRO)</span></li>
  <li>Orders split per status <span class="text-green-600 font-semibold">(PRO)</span></li>
  <li>Average units per order <span class="text-green-600 font-semibold">(PRO)</span></li>
  <li>Orders by time</li>
  <li>Orders chart</li>
  <li>Regions popularity</li>
  <li>Sales channel popularity</li>
  <li>Orders frequency distribution</li>
  <li>Payment provider popularity</li>
</ul>

<h3 class="mt-4 text-md font-semibold">Sales</h3>
<ul>
  <li>Average sales <span class="text-green-600 font-semibold">(PRO)</span></li>
  <li>Sales per channel <span class="text-green-600 font-semibold">(PRO)</span></li>
  <li>Net sales <span class="text-green-600 font-semibold">(PRO)</span></li>
  <li>Sales by time</li>
  <li>Sales by currency code</li>
  <li>Sales chart</li>
  <li>Refunds</li>
</ul>

<h3 class="mt-4 text-md font-semibold">Customers</h3>
<ul>
  <li>Average sales per customer <span class="text-green-600 font-semibold">(PRO)</span></li>
  <li>Customer lifetime value <span class="text-green-600 font-semibold">(PRO)</span></li>
  <li>New customers by time</li>
  <li>Repeat customer rate</li>
  <li>Customers chart</li>
  <li>Cumulative customers by time</li>
  <li>Retention customer rate</li>
</ul>

<h3 class="mt-4 text-md font-semibold">Products</h3>
<ul>
  <li>Top variants</li>
  <li>Top returned variants</li>
  <li>Products sold count</li>
  <li>Out of the stock variants</li>
</ul>

<h3 class="mt-4 text-md font-semibold">Marketing</h3>
<ul>
  <li>Top discounts</li>
</ul>

## Q&A

### Where is the source code?

This plugin is now behind the licence, so we cannot share the source code.

### I am interested, what I need to do?

As mentioned, this plugin is behind the licence. We offer two types of licences:
- subscription - recommended for people who create the store for their own, so for very low monthly cost you can have this functionality.
- lifetime - recommended for people who create the store for the client (so cannot spend money on monthly basis). For one price, you can get Store Analytics Pro forever.

We offer also 14-day free trial if you are not sure if you need this plugin - please reach us via labs@rsoftcon.com or go to https://medusa-plugins.com.
