#D365_Sales #D365  
**Table of contents**
- [[#Get started|Get started]]
	- [[#Get started#Sales|Sales]]
	- [[#Get started#Main terms|Main terms]]
	- [[#Get started#Copilot capabilities|Copilot capabilities]]
	- [[#Get started#Marketing lists|Marketing lists]]
	- [[#Get started#Campaign types|Campaign types]]
- [[#Set up and configure|Set up and configure]]
	- [[#Set up and configure#Currencies|Currencies]]
	- [[#Set up and configure#Docs|Docs]]
	- [[#Set up and configure#Security roles|Security roles]]
	- [[#Set up and configure#Access levels|Access levels]]
	- [[#Set up and configure#Copilot|Copilot]]
		- [[#Copilot#Summary and Recent changes|Summary and Recent changes]]
- [[#Manage leads|Manage leads]]
	- [[#Manage leads#Overview|Overview]]
	- [[#Manage leads#Create leads|Create leads]]
		- [[#Create leads#Manually creating leads|Manually creating leads]]
		- [[#Create leads#Quick create dialog box|Quick create dialog box]]
		- [[#Create leads#Converting email activities to leads|Converting email activities to leads]]
		- [[#Create leads#Bulk importing leads|Bulk importing leads]]
	- [[#Manage leads#Lifecycle|Lifecycle]]
	- [[#Manage leads#Qualify a lead|Qualify a lead]]
- [[#Opportunity|Opportunity]]
- [[#Product catalog|Product catalog]]
	- [[#Product catalog#Product catalog components|Product catalog components]]
	- [[#Product catalog#Currencies|Currencies]]
	- [[#Product catalog#Product configuration|Product configuration]]
	- [[#Product catalog#Product properties|Product properties]]
	- [[#Product catalog#Product bundles|Product bundles]]
	- [[#Product catalog#Defining related products|Defining related products]]
	- [[#Product catalog#Defining price list line items|Defining price list line items]]
	- [[#Product catalog#Product catalog settings|Product catalog settings]]
- [[#Relationships with relationship selling in D365 Sales|Relationships with relationship selling in D365 Sales]]
	- [[#Relationships with relationship selling in D365 Sales#Overview|Overview]]
	- [[#Relationships with relationship selling in D365 Sales#Sales accelerator|Sales accelerator]]
		- [[#Sales accelerator#Default filters|Default filters]]
	- [[#Relationships with relationship selling in D365 Sales#Sequences|Sequences]]
	- [[#Relationships with relationship selling in D365 Sales#Relationship analytics|Relationship analytics]]
	- [[#Relationships with relationship selling in D365 Sales#Predictive lead scoring|Predictive lead scoring]]
	- [[#Relationships with relationship selling in D365 Sales#Sales Navigator|Sales Navigator]]
- [[#Analyze Dynamics 365 sales data|Analyze Dynamics 365 sales data]]
	- [[#Analyze Dynamics 365 sales data#Out-of-box tools|Out-of-box tools]]
	- [[#Analyze Dynamics 365 sales data#Power BI|Power BI]]


# Get started
## Sales
[(More)](https://learn.microsoft.com/en-us/training/modules/sales-get-started/overview)
- **Sales Professional** - Ideal for enterprises that need a sales automation solution. 
- **Sales Enterprise** - Ideal for enterprises that need a sales automation solution with contextual insights and advanced customization capabilities.
- **Sales Premium** - Ideal for enterprises that need a sales automation solution, along with AI-driven insights that are powered by conversation intelligence, relationship intelligence, and more.
- **Microsoft Relationship Sales** - Ideal for enterprises that need to connect sales records with LinkedIn to enhance business processes with data about people, organizations, and relationships.
- **Microsoft Sales Copilot** - Ideal for enterprises that want sellers to use Microsoft 365 and Microsoft Teams to automatically capture, access, and register data into any customer relationship management (CRM) system, eliminating manual data entry. 
## Main terms

| Term                  | Definition                                                                                                                                                                                                                                                                                                                              |
| --------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Account               | An account represents a ==business or organization==. Occasionally, this account is a customer or a vendor. In some organizations, the account might be a different grouping, such as a family. Typically, an account has related contact records.                                                                                      |
| Activities            | An activity is a type of entity that offers ==tracking and scheduling== options. By default, the system has activities already set up, such as email, appointment, and phone call. An administrator can add more custom activities to meet other business needs.                                                                        |
| Assistant             | The assistant monitors your daily actions and communications. Additionally, it ==helps you== stay on top of your day with insight cards that display through the application to help provide actionable insights.                                                                                                                       |
| Business process flow | A business process flow is a type of automation in Microsoft Power Platform. The business process flow is placed on an entity form and offers users ==guidance and a predictable action plan== for gathering data. Administrators can add more automation based on triggers from the user's interaction with the business process flow. |
| Contact               | A contact represents a ==single individual==. Often, a contact has many related records, such as an account and activities.                                                                                                                                                                                                             |
| Customer              | Customers ==can be an account or a contact==. Typically, in a business-to-business scenario, this entity is an account. In a business-to-consumer scenario, this entity is a contact.                                                                                                                                                   |
| Opportunity           | Similar to a lead, an opportunity is a ==potential sales transaction==. Typically, an opportunity is a more viable prospect than a lead, and it contains more information and is tracked for a longer period of time.                                                                                                                   |
| Product catalog       | A product catalog is a ==collection== of records that interacts with opportunities, quotes, orders, and invoices ==to facilitate management== of products, price lists, discounts, and product families for sales transactions.                                                                                                         |
| Quote                 | A quote is a ==formal offer== for products or services that's proposed at ==specific prices== and related payment terms to a customer.                                                                                                                                                                                                  |
| Order                 | An order is a ==confirmed request== for the delivery of goods and services based on specified terms or a quote that a customer has accepted.                                                                                                                                                                                            |
| Invoice               | An invoice is an ==order== or record of a sales, including details ==about purchased products== or services that have been billed to the customer.                                                                                                                                                                                      |
| Sequence              | This feature helps enforce best practices by introducing a set of ==consecutive activities for sellers== to follow during their day.                                                                                                                                                                                                    |
| Timeline              | With this feature, you can provide a timeline of ==activities==, such as appointments, tasks, and emails, that are related to the current record.                                                                                                                                                                                       |
> [!note] Primary contacts
> Each account typically has one main contact that serves as the main point of contact for the account. You can set any contact that's associated with an account as the primary contact. After you define a **Primary Contact** for an account, ==their phone number and email address are displayed on the account record==.

## Copilot capabilities
[(More)](https://learn.microsoft.com/en-us/training/modules/sales-get-started/copilot)
- **Record summarization:** Provides you with a quick summary of your opportunity and lead records.
- **Recent changes:** Copilot summarizes any changes that were made to your lead, opportunity, and account records.
- **Meeting preparation:** Copilot helps you prepare for your upcoming meetings effortlessly, summarizing relevant information from the opportunity or lead records that are associated with the meeting.
- **Email assistance:** Copilot can help you compose professional-looking emails, summarize email conversations to add to your customer notes, and give you reminders to follow up on emails you haven't replied to.
- **News updates:** Copilot can help you stay current with the latest news about your accounts.
> [!tip]
> The simplest way to get started with Copilot in Dynamics 365 Sales is to tell it what you need. Copilot responds to various different commands. You can launch the Copilot pane, by selecting the Copilot Icon.

## Marketing lists
[(More)](https://learn.microsoft.com/en-us/training/modules/sales-get-started/in-app-marketing)
>You can use marketing lists to group similar accounts, contacts, or leads  together so that you can target them as part of marketing campaigns into a targeted marketing list.

Two types of marketing lists that you can create are:
- **Static** - Add and update list members manually.
- **Dynamic** - Add and update list members dynamically based on the search criteria that you set.

## Campaign types
[(More)](https://learn.microsoft.com/en-us/training/modules/sales-get-started/in-app-marketing)
- **Standard** - Use standard campaigns to manage the end-to-end process of a complete marketing campaign, including managing campaign and planning activities, distributing the activities to other team members, and tracking how the campaign did.
- **Quick** - Use quick campaigns to automatically distribute a single activity to selected accounts, contacts, or leads, or to a single marketing list.
> [!tip]
> Standard campaigns are typically implemented over a long period of time, whereas quick campaigns are immediate.

Marketing reports:
- **Campaign Activity Status** - Provides a summary for a single campaign.
- **Campaign Comparison** - Compares different campaigns to help identify your most and least successful campaigns.
- **Campaign Performance** - Tracks the progress and status of your campaigns.
> [!important] 
> To have the contact unsubscribe automatically when they select **unsubscribe**, you need to set up the application to do so automatically. In the **Sales Hub** app, go to the **App Settings** area. Under the **Sales Administration** group, select **Marketing Settings**. On the **Marketing Settings** page, set the **Set "Do Not Send Marketing Material" option when unsubscribe email is received** option to **Yes**.



#  Set up and configure

## Currencies
When setting up your currency settings, you can customize the following information:
- **Currency type** - Which currency, or currencies, you want to use.
- **Currency code** - Short form of the currency (for example, USD for United States dollar).
- **Currency precision** - Number of decimals that you want to use for the currency. You can add a value between 0 and 4.
- **Currency name** - Unless you selected a custom currency for **Currency type**, this column will be filled automatically.
- **Currency symbol** - Unless you selected a custom currency for **Currency type**, this column will be filled automatically.
- **Currency conversion** - The value of the selected currency in terms of one US dollar. Make sure that you update this value frequently, as required, to avoid inaccurate calculations in your transactions.

## Docs
[(More)](https://learn.microsoft.com/en-us/training/modules/configure-dynamics-365-sales/document-management)
When you use SharePoint Online with customer engagement apps, you can:
- **Create, upload, view, and delete documents** that are stored in SharePoint from within customer engagement apps.
- **Use the SharePoint document management abilities** within customer engagement apps, such as checking in or checking out the document and changing document properties.
- **Enable noncustomer engagement apps users**, such as customers who want to review a bid, to directly access the SharePoint documents (if they have the appropriate permissions).

> [!important] 
> By default, document management isn't set up in new environments. If your organization hasn't deployed document management, when a system administrator signs in, an alert message will be displayed to enable server-based SharePoint integration.
> ![[Pasted image 20240822153430.png]]
> If the message doesn't appear, you can still set up the functionality through the [Power Platform admin center](https://admin.powerplatform.microsoft.com/). In the Power Platform admin center, select an environment that you want to set up, go to **Settings > Integration > Document management settings**, and then select **Enable Server-Based SharePoint Integration**. This action will direct you to a configuration wizard that will assist you in setting up server-based SharePoint integration.

When the **Documents** tab opens, the **Document Associated Grid** will display, which will provide you with the following options:
- **New** - Allows you to create a new document directly from within the window. You'll be able to create a Word document, Excel spreadsheet, OneNote notebook, or PowerPoint presentation. You can also create a new folder to store documents.
- **Upload** - Allows you to upload an existing document directly to the SharePoint site.
- **Document Location** - Allows you to specify which document location that you want to view documents from. You might have multiple locations set up for different types of documents.
- **Open Location** - Lets you open the SharePoint document location directly from the subgrid so that you can take advantage of all available options.
- **Add Location** - Allows you to add an extra document location for storing documents.
- **Edit Location** - Lets you make changes to the existing document location that you're working with.
- **Refresh** - Refreshes the document location.

## Security roles
[(More)](https://learn.microsoft.com/en-us/training/modules/configure-dynamics-365-sales/4-security-roles)
>Security roles in Dynamics 365 Sales are a matrix of security privileges (row-level) and access levels (task-based) for different tables. Different tabs are available based on functionality within this security matrix. People can have more than one security role. These roles are cumulative, so all permissions will be based on all roles that are assigned to the user.

Privileges are the securities that define what action a user can take in the system, such as:
- Create
- Read
- Write
- Delete
- Append
- Append to
- Assign
- Share

## Access levels
[(More)](https://learn.microsoft.com/en-us/training/modules/configure-dynamics-365-sales/4-security-roles)
> Access levels show the **level at which a user can interact with rows within a given table**. The portion of the circle that is filled illustrates the levels. The levels are **None, User, Business Unit, Parent-Child Business Unit, and Organization**. Click the circle to change the level. Each click will change the fill or color. Click the circle until it shows the level that you want.
- **User (basic)** - This level gives access to rows that the user owns or to anything that is shared with the user or team to which the user belongs. Use this setting if you want the user to access their own rows only. You wouldn't want to let salespeople delete other salespeople’s accounts or leads.
- **Business Unit (local)** - This level allows access to the data of other users in a business unit. A business unit must be set up within Dynamics 365 and can be a hierarchy of a department. Sales managers would want to view all their subordinates’ rows.
- **Parent: Child Business Units (deep)** - This level gives access to all business units that the user belongs to and to any business units that are subordinate to their business unit.
- **Organizational (global)** - A user with this level has access to all rows in the organization. If you have a salesperson who is able to add products from any level of the organization, you want to give them access to all organizational products, not only the ones that are available for their business unit.

## Copilot
[(More)](https://learn.microsoft.com/en-us/training/modules/configure-dynamics-365-sales/copilot)
Copilot is configured in the **App Settings** area of the **Sales Hub** app, Under **General Settings**, select **Copilot**.
The Copilot Configuration screen contains three sections:
- Setup
- Opportunities
- Leads
Under **Enable Copilot for**, select a global setting that you want to apply for all Sales apps and then override the setting at the app-level. For example, if you want to enable Copilot only for the Sales Hub app, select **Off** for **All Dynamics 365 Sales apps** and then select **On** only for the Sales Hub app.

### Summary and Recent changes
>For both Summary and Recent changes, you can define a maximum of 10 fields that you want to use. You'll need to make sure that you have at least four selected.

By default, for **Opportunities** the following fields are enabled for both summarization and recent changes:
- **Opportunity**
    - Est. revenue
    - Customer Need
    - Proposed Solution
    - Est. close date
- **Related Account**
    - Annual Revenue
    - Primary Contact
- **Related Contact**
    - Job Title
- **Opportunity Product**
    - Product Name
- **Competitor**
    - Strength
    - Name

For **leads**, the fields enabled for summarization and recent changes are as follows:
- Lead
    - Topic
    - Lead Source
    - Rating
    - Preferred Method of Contact
    - Source Campaign
    - Created on
- Related Account
    - Primary Contact
    - Annual Revenue
- Competitor
    - Strength
    - Name

# Manage leads

## Overview
[(More)](https://learn.microsoft.com/en-us/training/modules/manage-leads-dynamics-365-sales/1-leads-overview)
>A _lead_ is someone with an interest in what you are selling. A lead might be an existing client, or someone that you have never done business with before.

>Leads are considered temporary records. The goal of a lead is to determine the viability of being a customer. This is referred to as _lead qualification_.

The following image shows an example sales process from beginning to end:
![[Pasted image 20240822163833.png]]

## Create leads
### Manually creating leads
Leads can be manually created in Microsoft Dynamics 365 by using the Sales Hub app. In the app, navigate to **Leads** > **New**. The **New Lead** page appears, where you can enter details like the lead's name, contact information, and company information. When you create a lead, **Topic** and **Last Name** are the only required columns.

### Quick create dialog box
To open the **Quick Create: Lead** dialog box, select the **New** button on the navigation bar. You also use this dialog box when you create new leads from the **Related** tab on account and contact records. The **Quick Create: Lead** dialog box doesn't include columns for address information. It just includes columns for the most essential details about a lead, like the source of the lead, and the lead's first and last names, company, and email and phone contact information.

### Converting email activities to leads
Another way to create leads in Dynamics 365 Sales is to convert emails to leads. You can convert an email to a lead directly in the sales application.

### Bulk importing leads
When you're viewing leads, you can import new leads by using the command bar. Leads can be imported in two formats: **Microsoft Excel files or comma-separated values (CSV) files**. 
When you import a file that includes leads, you must **make sure that the columns in the file can be mapped to specific columns** in Dynamics 365 lead records. After you select the file to import, you'll be asked to review the mappings.
> [!tip]
> Sometimes, it's easier to export a template that has the Dynamics 365 column labels, add the data that you want to import in the exported template, and then import the template. This approach helps guarantee that all the columns are correctly matched. It also helps save you time.

## Lifecycle
Here are some of the lead-related views that Microsoft Dynamics 365 includes:
- **Open Leads-** All leads that are currently open, regardless of who the lead owner is.
- **Closed Leads-** All leads that are closed. Both qualified and disqualified leads are included.
- **All Leads-** All open and closed leads.
- **My Open Leads-** All the open leads that are assigned to the signed-in user.
- **Leads opened last week-** All leads that were created last week.
- **Leads opened this week-** All new leads created during the current week.

## Qualify a lead
**Potential customer** column in the opportunity record can be set to either an account record or a contact record. If the lead is associated with an existing customer, the existing customer that's defined for the lead will be used as the customer for the opportunity. If the lead is a brand-new customer, an account and/or contact record must exist for the lead before an opportunity can be created.
![[Pasted image 20240823161141.png]]
The following values on the **Lead** page control the outcome of the qualification process:
- **Title:** This value becomes the title of the opportunity that's created.
- **Name:** If this value is entered, it becomes the full name of the new contact.
- **Company:** This value becomes the name of the newly created account using the company name.
> [!note]
> Other data, like the customer's budget from the lead, is mapped to the new opportunity.

# Opportunity
[(More)]([https://docs.microsoft.com/en-us/learn/modules/manage-opportunities-dynamics-365-sales/](https://docs.microsoft.com/en-us/learn/modules/manage-opportunities-dynamics-365-sales/))

Typical sales lifecycle:
![[Pasted image 20240823171614.png]]
Here's a description of some of the main information that can be included for an opportunity:

| Information            | Description                                                                                                                                              |
| ---------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Stakeholders           | Contacts in Dynamics 365 who have a vested interest in the opportunity. Stakeholders can include project managers, board members, lawyers, and sponsors. |
| Sales team             | Internal team members who will be involved in converting the opportunity to a sale.                                                                      |
| Competitors            | Any external competitors that you might be competing against for the deal.                                                                               |
| Pricing information    | The price lists that will be used and the calculation method that will be used to estimate the value of the opportunity.                                 |
| Opportunity line items | The specific products and services that are being suggested to the customer as part of the solution.                                                     |
Revenue information can be provided by the user or calculated by the system. Set the **Revenue** column to one of the following values:
- **User Provided:** The user manually enters the estimated revenue from the opportunity (Default).
    - A Dynamics 365 price list doesn't have to be added to the opportunity.
    - Line items for individual products don't have to be added to the opportunity.
    - The Dynamics 365 product catalog isn't required.
- **System Calculated:** The estimated revenue from the opportunity is automatically calculated based on the individual line items that are added to the opportunity.
    - A Dynamics 365 price list must be added to the opportunity.
    - Line items for products can be added either from current products in the Dynamics 365 product catalog or as write-in products. Product line items include the following information:
        - **Existing Product or Write in Product:** Enter the name of the product that's being added.
            - Existing products use the name that's provided in the product catalog.
            - A name can be defined for write-in products when they're added
        - **Unit:** Enter the unit that the product should be sold in. Examples include each, pack, and case.
        - **Price Per Unit:** Enter the amount to charge per unit that's sold.
        - **Quantity:** Enter the number of units to include.
        - **Manual Discount Amount:** Enter the amount of any manual discounts that should be applied.
        - **Tax:** Enter any sales tax information.

Here are some of the opportunity-related views that Microsoft Dynamics 365 includes:
- **My Open Opportunities:** All the open opportunities that are assigned to the signed-in user.
- **Closed Opportunities:** All opportunities that have been closed. Both won and lost opportunities are included.
- **Lost Opportunities:** All closed opportunities that were identified as lost.
- **Recent Opportunities:** All opportunities that were recently created.
- **Won Opportunities:** All closed opportunities that were identified as won.

![[Pasted image 20240823175117.png]]
1. **Metrics**: View the key metrics or KPIs that you want to track. Select a metric to view the underlying data.
2. **Charts**: Get a visual representation of the pipeline.
3. **Editable grid**: View a list of opportunities and edit them inline. Select any linked column to view and edit details in the side panel. Select the three-dot menu against an opportunity to perform common actions, such as closing the opportunity as won or lost, or reopening the opportunity.
4. **Side panel**: View and quickly edit details of the linked record. You can also navigate from one object to another in the side panel. For example, while you're looking at the opportunity, you can select a contact to view their details, quickly make updates, and then return to the opportunity.

Opportunities can be in one of three statuses:
- Open – The opportunity is currently being pursued.
- Won – The opportunity was won.
- Lost – The opportunity was lost.
	- Canceled
    - Out-sold

| Phase   | Table                                        | Description                                                                                                                                                                                                                                                                                                                        |
| ------- | -------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Qualify | Lead (Lead to Opportunity Sales Process BPF) | If your lead isn't already in Dynamics 365 Customer Engagement apps, you must first create the lead in the system. After you've determined that your lead is interested in your solution or product and has the appropriate purchasing power, you can qualify the lead. When you qualify a lead, it's converted to an opportunity. |
| Qualify | Opportunity (Opportunity Sales Process BPF)  | When you start from an opportunity, you must identify the target account and contact. You can then qualify the opportunity by collecting more information.                                                                                                                                                                         |
| Develop | Opportunity                                  | During this phase, you identify stakeholders, competitors, and sales team members, and come up with a proposed solution.                                                                                                                                                                                                           |
| Propose | Opportunity                                  | During this phase, you develop a proposal and present it to your potential customer.                                                                                                                                                                                                                                               |
| Close   | Opportunity                                  | During this phase, you must work with the customer to reach a decision within the specified timeframe and close your opportunity as either won or lost.                                                                                                                                                                            |

# Product catalog
[(More)](https://learn.microsoft.com/en-us/training/modules/manage-organize-product-catalog-dynamics-365-sales/1-product-catalog-overview)
## Product catalog components

The Dynamics 365 product catalog consists of four components:
- **Unit groups:** A unit group defines how a product is packaged for sale. Among other values, it defines the units of measure that the product or service is sold in.
- **Products:** A product represents the type of product that a company might keep in inventory, a custom-built product, or a service provided to a customer.
- **Price lists:** A price list is a set of prices that are charged for products under specific circumstances.
- **Discount lists:** A discount list lets organizations offer products or services at different prices, depending on the quantity bought. 

## Currencies
[(More)](https://learn.microsoft.com/en-us/training/modules/manage-organize-product-catalog-dynamics-365-sales/2-currencies-and-currency-management)
Three components help support the Dynamics 365s multi-currency solution:
- **Base currency-** The base currency is the currency that other currencies are quoted in.
- **Transaction currency-** The transaction currency is the currency that's used for a specific transaction.
- **Exchange rates-** An exchange rate represents the number of units of a transaction currency that equals one unit of the base currency.

## Product configuration
[(More)](https://learn.microsoft.com/en-us/training/modules/manage-organize-product-catalog-dynamics-365-sales/3-define-products)
When you define a product, you can include the following information:

|Column|Description|
|---|---|
|Name|Enter the name of the product to use when the product is added to price lists, opportunities, work orders, orders, and so on.|
|Product ID|Specify the ID of the product. This ID can then be referenced when the product is added to other Microsoft Dynamics 365 records.|
|Parent|This column is used when the product is associated with a product family. The value can't be changed after the record is saved.|
|Valid From, Valid To|Specify the date range when the product can be added to items.|
|Description|Enter a brief description of the product. You can use this column to provide more details.|
|Unit Group|Define the unit group that defines quantity information that's related to how the product can be sold.|
|Default Unit|Specify the default unit that to use for the product, based on the unit group.|
|Default Price List|Define the price list that to use for this product by default. Although a product can be associated with multiple price lists, it can have only one default price list.|
|Decimals Supported|Define the number of decimal places that can be used when the product is added to items. The precision of the **Quantity** column in the quote, order, or invoice product record is validated against the value in this column if the product doesn't have an associated price list.|
|Subject|Associate this product with a subject. You can use subjects to categorize your products and filter reports.|

> [!important]
> By default, product records are created in a draft state. While a product is in a draft state, sales staff can't add it to items like opportunities, quotes, or orders. When you're ready to sell a product, you must publish it.

## Product properties
[(More)](https://learn.microsoft.com/en-us/training/modules/manage-organize-product-catalog-dynamics-365-sales/4-product-families)
>Another advantage of product families is that you can define properties to help distinguish products. For example, a property can be used to offer size or color options for shirts that belong to the same family.

When a property is created, you must define the following details:
- **Name:** Enter the name of the property that will be presented to users when they set it.
- **Read-Only:** Specify whether users can edit the property.
- **Required:** Specify whether a value must be defined for the property.
- **Hidden:** Specify whether the property will be hidden to users when it's consumed.

## Product bundles
[(More)](https://learn.microsoft.com/en-us/training/modules/manage-organize-product-catalog-dynamics-365-sales/4-product-families#:~:text=items%20sub%2Dgrid.-,Product%20bundles,-A%20bundle%20is)
>A bundle is a collection of products that are sold as a single unit. From within a bundle, users can see all the products that are included in the bundle.

## Defining related products
[(More)](https://learn.microsoft.com/en-us/training/modules/manage-organize-product-catalog-dynamics-365-sales/4-product-families#:~:text=Defining%20related%20products)
>Related products can be defined for individual product records or product bundles, but they can't be defined for a product family. To add a relationship, select **Product Relationships** on the **Related** tab. Then select the **Add New Product Relationship** button.

When you define a product relationship, you must include the following information:
- The product that the relationship is being created for.
- The related product the product is being associated with.
- The type of relationship. You can select _Up-Sell_, _Cross-Sell_, _Substitute_, or _Accessory_.
- The direction of the relationship:
    - **Uni-directional:** The relationship is available only from the product.
    - **Bi-directional:** The relationship is available from both the product and the related product.

## Defining price list line items
[(More)](https://learn.microsoft.com/en-us/training/modules/manage-organize-product-catalog-dynamics-365-sales/5-price-lists#:~:text=Defining%20price%20list%20line%20items)
>After you've saved a price list for the first time, you can define individual price list line items by selecting the **Add new price list item** button on the **Price list items** tab. When an item is first added, you can define the following values:
- **Price List:** Specify the price list to add the line item to.
- **Product:** Define the product from the product catalog to associate the line item with.
- **Unit:** Define the unit of measure to use with the line items, based on the unit group that's associated with the product.
- **Discount List:** Define the discount list to use if the line item requires any volume discounts.
- **Quantity Selling Option:** Define whether the item can be sold whole or in fractional amounts.

>Pricing information for each line item is defined on the **Pricing** tab on the **Price List Item** page. The first and most important column that you must define is the **Pricing Method** column. This column defines the actual price of the item for this price list. The following options are available:
- **Currency Amount:** Select this option to ignore a product's list price in the product catalog and manually enter a different price for this price list.
- **Percent of List:** Select this option to calculate a product's price on the price list as a percentage of its list price.
- **Percent Markup - Current Cost:** Select this option to add a percentage markup on top of the current cost that's entered in the product catalog.
- **Percent Margin - Current Cost:** Select this option if the price that's offered on the price list should yield a percentage margin of the current cost.
- **Percent Markup - Standard Cost:** Select this option to add a percentage markup on top of the standard cost that's entered in the product catalog.
- **Percent Margin - Standard Cost:** Select this option if the price that's offered on the price list should yield a percentage margin of the standard cost.

## Product catalog settings
[(More)](https://learn.microsoft.com/en-us/training/modules/manage-organize-product-catalog-dynamics-365-sales/6-configure-product-catalog)
The product catalog settings are accessed for the App settings area in the application. There are multiple settings that can be modified. In the general settings section, you can modify the following settings:
- **Create product is active state**: Typically, products are created in an inactive state and need to be individually activated. Specifies if products should be created in the active state. When enabled, products are automatically activated when they're created. (Only applies to products that aren't associated to a product family.)
- **Allow selection of default price list**: Set whether the default price list for an opportunity should be selected via an inbuilt rule. (Based on the default price list defined for territories.)
- **System pricing calculation**: Defines whether to use system pricing calculation or if you want to use custom pricing using a plug-in.
- **Make price list optional**: Allow individual line items to be created in opportunities, quotes, orders, and invoices, on without an associated price list.
- **Max number of products in a bundle**: Specifies the maximum number of products a bundle can have. By default, that number is 15.
- **Max number of properties of a product bundle**: Specifies the maximum number of properties a product or bundle can have. Dy default, the number is 50.
- **Discount calculation method**: Specifies if discounts should be applied to each unit or for each line item. By default, it's set to Line item.

# Relationships with relationship selling in D365 Sales 
## Overview
[(More)](https://learn.microsoft.com/en-us/training/modules/manage-relationships-social-selling-dynamics-365-sales/1-overview)
**Dynamics 365 Sales Insights**: Helps sales professionals to build strong relationships with customers, take actions based on insights, and close sales faster. Sales Insights includes:
- **Relationship analytics**: Gathers relevant information from throughout the Dynamics 365 database to create a graphical display of key performance indicators (KPIs) and activity histories.
- **Predictive lead scoring**: Helps you to focus on revenue generation efforts by providing scores to prioritize efforts on quality leads.
- **Predictive opportunity scoring**: Helps you to focus on revenue generation efforts by providing scores to prioritize efforts on quality opportunities.
- **Notes analysis**: Monitors notes that you enter regarding a recent meeting or discussion with your customer to provide intelligent suggestions.
- **Talking points**: Displays topic ideas such as sports, vacation, family, and entertainment, to help you start a conversation with your customer.
- **Who knows whom**: Provides details such as names and email addresses of your colleagues who know a lead that you interact with.

By using the **Sales accelerator**:
- Sellers can prioritize their customer list in a fast and easy way by using an intelligent work list. The work list helps sellers reach out to the next best lead or opportunity by displaying relevant sales information and customer context that's available immediately, which helps make every communication more successful.
- The sequence designer allows you to create and manage your own sequences.
- Sales managers can use the sequence designer to configure sequences of activities that define steps to help sellers:
    - Prioritize their activities for the day,
    - Be productive in their jobs,
    - And focus on selling.

With **LinkedIn Sales Navigator** integration, sellers can:
- Get headline information, recent activities, news, and job changes when viewing the customer record in Microsoft Dynamics.
- Use icebreakers to identify commonalities between you and your prospects.
- Ask for an introduction to the lead from anyone within their network or anyone in your organization who might be connected to the lead.
- Get one-click access to LinkedIn InMail and increase your probability of reaching your buyer.

## Sales accelerator
[(More)](https://learn.microsoft.com/en-us/training/modules/manage-relationships-social-selling-dynamics-365-sales/sales-accelerator)
The sales accelerator is an engagement platform that helps a sales team understand customers' needs and respond in the following ways:
- Engage with customers by using multiple channels within one workspace.
- Minimize the time spent on searching for the next best customer to reach out to.
- Gather information from multiple sources and let sellers focus on how to best approach their customers.
- Sell smartly by building a strong and prioritized pipeline, offering context, and surfacing automated recommendations throughout a sales sequence that helps to expedite the sales process.

### Default filters
The following filters are available by default in the sales accelerator:
- **Unopened**: View records that weren't opened or read.
- **Followed**: View records that you're following.
- **Due by**: Filter records according to the time that a task must be completed for a record. The following options are available:
    - **Today**: View records with pending tasks that weren't completed today.
    - **From tomorrow**: View records with pending tasks that are to be completed tomorrow.
    - **Overdue**: View records with pending tasks that weren't completed on time.
- **Record type**: These filter options are the record types that the sales accelerator is configured for. You can select all options to view all records, or you can select an individual type to view only the records of that type.
- **Activity type**: These filter options are **Phone calls**, **Email messages**, **Tasks**, and **Meetings**. You can select all or any specific option to filter the records to display in the work list.

## Sequences 
[(More)](https://learn.microsoft.com/en-us/training/modules/manage-relationships-social-selling-dynamics-365-sales/sales-accelerator#:~:text=their%20own%20from.-,Create%20sequences,-The%20easiest%20way)
Sequence steps are categorized into the following four groups:
- **Steps**: A step in a sequence is an engagement task that a seller performs for sales outreach, such as sending an email (manual or automated), making a phone call, or completing a task. 
- **Conditions**: The condition step in a sequence determines the next course of action that the sequence will take after the condition is either met or not met, based on the completed activity. Examples of conditions include links being clicked, emails being opened, a reply and more.
- **Commands**: The command step in a sequence determines the next course of action according to the value given in the field or stage of a business process. Examples of commands include advancing to another sequence or updating a field on a record.
- **LinkedIn**: The LinkedIn activity step in a sequence allows sellers to diversify their day-to-day activities by including social selling functions. You can use LinkedIn's vast network with recommended actions that your sellers can take to build deeper connections.

## Relationship analytics
[(More)](https://learn.microsoft.com/en-us/training/modules/manage-relationships-social-selling-dynamics-365-sales/3-manage-relationship-health-with-sales-insights#:~:text=based%20add%20on.-,Relationship%20analytics,-Relationship%20analytics%20provides)
![[Pasted image 20240824012219.png]]
1. **Summary**: Provides metrics and key performance indicators (KPIs) that are computed from activities of current and past years.
    - **Call comparison**: Defines how the number of calls you placed to the customer compares with the number they placed to you.
    - **Hour's comparison**: Defines how much time your sellers have invested compared to the contact.
    - **Response comparison**: Defines how long it takes you to respond to communication compared to the contact.
    - **Email response comparison**: Defines how long it takes you to respond to emails vs the customer.
2. **Relationship health**: Display the overall health of your relationship with the customer based on opportunity and activity data. It also displays how the current relationship status is trending.
3. **Customer interactions**: Compares the number of interactions initiated by your sellers to the number of interactions initiated by the contact.
4. **Hourly investment**: Compares the overall number of hours spent by your sellers on emails, phone calls, meetings, and tasks with the contact, to the number of hours spent by the contact.
5. **Response Time**: Compares the average time it takes for sellers to respond to emails from this contact to the average time it takes this contact to respond to our emails.
6. **Email send/receive ratio**: Compares the ratio of the number of emails sent by you and received by the customer, to the number of emails sent by the customer and received by you.
7. **Relationship activities**: Provides a detailed look at activities over 90 days, broken down by date and activity type such as emails sent, emails received, meetings sent, meetings received, phone calls made, and phone calls received.

## Predictive lead scoring
[(More)](https://learn.microsoft.com/en-us/training/modules/manage-relationships-social-selling-dynamics-365-sales/3-manage-relationship-health-with-sales-insights#:~:text=phone%20calls%20received.-,Predictive%20lead%20scoring,-This%20model%20assigns)
![[Pasted image 20240824012439.png]]
1. **Lead score**: Displays the basic information of a lead such as lead score, lead grade, and lead score trend, to help you avoid going back to the My Open Leads Scored view to see basic information.
2. **Lead score over time**: Chart highlighting the leads score over the past month.
3. **Score improvers**: Displays the list of reasons that are affecting the lead score in a positive way. This helps you to analyze and consider the lead for converting into an opportunity.
4. **Score harmers**: Displays the list of reasons that are affecting the lead score in a negative way.

## Sales Navigator
[(More)](https://learn.microsoft.com/en-us/training/modules/manage-relationships-social-selling-dynamics-365-sales/5-sales-navigator)
The **LinkedIn Sales Navigator Lead** control shows information about a LinkedIn member profile. This control has the following sections, which you can choose to show or hide:
- **Top Card**: Shows information about the person like name, headline, and more. Additionally, it provides capabilities to message or save the person as a lead in Sales Navigator.
- **News (Icebreakers)**: Shows the person's highlights, activities, conversation starters, and more.
- **Connections (Get Introduced)**: Shows the mutual connections and allows for a warm introduction to the person.
- **Related Leads**: Shows potential Sales Navigator leads who are similar to the target person and might represent the relevant stakeholders around them. On a sales scenario, this insight is crucial to identify the potential decision-makers for a deal.

The **LinkedIn Sales Navigator Account** control shows information about a LinkedIn company profile. This control has four modules, which you can choose to show or hide:
- **Top Card**: Shows information about the company like company name, industry, location, and more. Additionally, provides capabilities to view the related account and save it in Sales Navigator.
- **News**: Shows the latest news of this company.
- **Connections**: Shows relevant connections for this company that can establish a first contact.
- **Kind Key People**: Shows the recommended potential leads in this company that might be opportunities open for the next deal.

# Analyze Dynamics 365 sales data
## Out-of-box tools
[(More)](https://learn.microsoft.com/en-us/training/modules/analyze-dynamics-365-sales-data/3-out-of-the-box-tools)
Microsoft Dynamics 365 has two commonly used features that meet the needs of these users:
- **Charts:** Charts provide visual insights into an organization's or user's most important data and information. Each table has several predefined charts that can be used to quickly consume big picture data.
- **Dashboards:** Dashboards let users see, at a glance, the most important information that they need to make business decisions. Dashboards can consist of charts, lists, and other resources, like external webpages. Dynamics 365 includes several preconfigured dashboards that help shed light on the most important information. These preconfigured dashboards can be changed, and custom dashboards can be created.

Here are some of the types of components that can be added to a dashboard:
- **Chart:** This component shows a Dynamics 365 chart. If you add a chart to a dashboard, you must define the following properties:
    - The table to use
    - The view that defines the data that's shown in the chart
    - The specific chart to show
- **List:** This component shows a specific Dynamics 365 view. If you add a list to a dashboard, you must define the following properties:
    - The table to use
    - The specific view to show
- **IFrame:** This component shows information for a webpage.
- **Web resource:** This component shows information for a web resource that has been added.
- **Assistant:** This component shows the Assistant.

## Power BI
[(More)](https://learn.microsoft.com/en-us/training/modules/analyze-dynamics-365-sales-data/4-power-bi)
>Microsoft Power BI is a suite of business analytics tools that deliver insights throughout your organization. Power BI helps connect to hundreds of data sources, simplifies data preparation, and drives ad-hoc analysis. By using the tools that Power BI provides, you can produce beautiful reports and then publish them so that your organization can consume them on the web and across mobile devices.

Because Power BI connects to Dynamics 365 and part of the application, there are some limitations that you should consider when you're deciding whether to use Power BI:
- **Power BI doesn't run in the context of records or users:** Unlike charts and dashboards, Power BI doesn't run in the context of a record or user. Although the functionality can be extended so that it includes links to individual records, this capability isn't available natively.
- **Data updates occur hourly or daily:** Power BI doesn't show a real-time view of Dynamics 365 data. The data is updated at specific intervals that depend on your pricing tier.

The following **Power BI template** apps are available to analyze your sales data in Dynamics 365 Sales:
- Sales Analytics for Dynamics 365 Sales
    As a sales manager, use this dashboard to perform the following tasks:
	- Monitor the sales pipeline, sales leaderboard, and top deals.
	- Analyze pipeline performance, won/lost deals, and lead closure.
- Process Analytics for Dynamics 365
	As a sales enablement manager, use this template app to perform the following tasks:
	- Track business process performance.
	- Create custom dashboards that focus on just one business process.

