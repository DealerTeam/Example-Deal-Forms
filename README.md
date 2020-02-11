# Example Deal Forms
Printable forms you can use to prepare or extend printed documents from Deals.
## Getting Started
These instructions will walk you through installing the pages and customizing them to meet your needs.
### Installing Pages
1. Open the Developer Console under the settings gear

2. Under the File > New menu select Visualforce Page

3. Enter a descriptive name (e.g. DealQuoteCustom) and select ok

4. Paste the contents of the example page and save (File > Save)

### Viewing Pages
To view your page(s) you will need to pass the DealID parameter.


1. Click the App Launcher icon

2. Enter Deals in the search area.

3. Click Deals.

4. Select the Deal # to open up the deal.

5. Copy the unique identifier from the URL between the slashes. **a0N1F000001xTneUAE** is the DealId in the example below. ````https://velocity-dream-6454-dev-ed.lightning.force.com/lightning/r/dealer__Deal__c/**a0N1F000001xTneUAE**/view````

6. Browse to your page appending the DealID.
````https://velocity-dream-6454-dev-ed--dealer.visualforce.com/apex/DealQuoteCustom?id=a0N1F000001wlADUAY````

### Adding Pages to Forms
Reference the following help article to upload the form(s) to your org:
[Upload Visualforce Forms](https://help.dealerteam.com/System_Administration/System_Administrator_Guide/Upload_Visualforce_Forms)

## Customizing Pages
The pages can be customized to meet your needs. Outlined below are a few key areas.

###### Logo
The logo will display from the Location that is selected in the deal.
```HTML
<apex:image id="businessLogo" url="/{!dealW.logoURL}" />
```
###### Form Name
The default form name is **Quote**. To replace do a search for ````Quote```` and replace with a different name.

```HTML
<h1>Quote</h1>
```
###### Terms & Conditions
To update the terms do a search for ````Terms```` and make any necessary changes.

```html
<!-- Terms -->
```