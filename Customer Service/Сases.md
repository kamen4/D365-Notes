 #D365_CS #D365 
## Get started
[(More)](https://learn.microsoft.com/en-us/training/modules/get-started-with-dynamics-365-for-customer-service/1-overview)
### Introduction
![[Pasted image 20240829142039.png]]

### Types of records
**Cases**: Cases are the fundamental record type in service management and represent a single incident of any requested service. Different organizations might use different terms to refer to cases: _incidents_, _tickets_, _service requests_, and so on.

**Activities**: Interactions between a business and its customers that are considered important enough to track in Customer Service are known as _activities_. Activities can be associated with many kinds of records in Customer Service. You can open the record and find the activities under **Closed activities** or **Open activities**.
- Closed activities are those that are marked as completed.
- Open activities either aren't marked as completed or are waiting for completion at a different date and time.

**Entitlements**: Entitlements can be used to specify how much support services a customer is entitled to. For example, a customer's entitlement in Customer Service might allot 10 support cases that the customer can use at their discretion.

**Entitlement channels**: Entitlement channels can be used to specify the type of service a customer is entitled to. Out of the box, there are six entitlement channels:
- Phone
- Email
- Web
- Facebook
- Twitter
- IoT

**Knowledge Base articles**: The Knowledge Base in Customer Service is a repository of informational articles that help customer service representatives resolve cases. In some organizations, the information in the knowledge base helps employees not only resolve issues but also ask follow-up questions.

**Resolution activities**: After all the activities for a case are resolved, the case itself can be resolved. After the case is resolved, an activity of the **Resolution Activity** type is created. This activity is found in the closed activities associated with a case. Resolution activities show the case's resolution and how much time was spent on the case.

**Queues**: A queue is a place to organize and store activities and cases that are waiting to be processed.

**Products**: Products in the Microsoft Dynamics CRM Product Catalog can be related to a customer service case. Therefore, they can help provide a more detailed view of cases, resolutions, and customer feedback at a product level.

**Service level agreements**: Service level agreements (SLAs) are a way of tracking and defining what should happen when a case is opened. You can track things like when a support engineer first takes a case and how long it takes to resolve the case. You can also send emails based on specific warning and failure timelines.

### Modern customer journey
![[Pasted image 20240829165353.png]]With the advent of self-service capabilities, customers can now start educating themselves by using any of these resources:
- Power Pages with an interactive bot
- Live chat capability
- SMS communication
- Interactive kiosks
- A mobile app deployed by the customer's organization
- Remote sharing of screens between a service agent and the customer
- Any number of social networks, including Facebook and Twitter

 In general, the modern service company must consider the following:
- **Social media**: Customers are highly active on social media. They don't just leave comments about the things they like. They also comment, loudly, about what they don't like. What's more, many of their friends—your potential customers—are listening to those comments and forming their own opinions of your company.
- **Company size**: Companies often want to target both small and enterprise customers through the same set of channels.
- **Support for contract and non-contract customers**: Everyone gets support, not just those with service level agreements (SLAs). Again, you don't know where new customers are coming from.
- **Fast response times**: Customers expect fast response times. If you can't give them a timely response, they go elsewhere, maybe even to your competitors, who might have a better support channel in place.
- **On-site support**: Sometimes, customers can't be helped online. In this case, they often expect the service company to visit them at their place of business or in the field to resolve an issue.

## Managing cases
[(More)](https://learn.microsoft.com/en-us/training/modules/managing-cases-with-dynamics-365/)
### Case management overview
>A case typically represents a situation or incident that's reported by a customer and that requires a resolution. Cases are designed to track the process from the initial intake of an incident, through the remediation process, to the final resolution. From a customer service standpoint, a case can represent several items. Here are some common examples:

Here are some of the most commonly used components:
- **Cases:** A case represents a single incident of service. In other words, it represents anything, in the context of a customer interaction, that requires some type of resolution or answer. Multiple cases can be associated with a single customer at any time.
- **Activities:** An activity typically represents an interaction with a customer, like a phone call. Multiple activities can be associated with a single case.
- **Entitlements:** Entitlements specify the amount of support services that a customer is entitled to. Think of them as support contracts.
- **Knowledge articles:** The knowledge base is a repository of informational articles that help customer service representatives resolve cases.
- **Queues:** A queue is a place to organize and store activities and cases that are waiting to be processed.
- **Service level agreements (SLAs):** SLAs are a way to track and define what should happen when a case is opened, like how long it should take to respond to a customer.
- **Record creation and update rules:** Record creation and update rules can be applied to different activity types to automatically create Dynamics 365 records.
- **Routing rules:** Routing rules are applied to cases to automatically route them to a specific queue or user.
- **Business process flows:** A business process flow represents a guided process that has different stages and steps that are used to resolve a specific item, like a case.

### Case creation and lifecycle
Out of the box, the following types of Dynamics 365 activities can be converted to cases:
- Appointments
- Campaign Responses
- E-mails
- Faxes
- Letters
- Phone Calls
- Service Activities
- Tasks
- Social Activities


> [!important]
> Many organizations use activities to track what has been done against a case. These activities might be phone calls that were placed to the customer, tasks that needed to be completed and more. To ensure that you're addressing these activities as appropriate, when you close a case with open activities, you see a message with the following actions:
> - A link with the number of open activities. You can select the link to view the open activities associated with the case on a tab your administrator has configured.
> - **Confirm**: If you select Confirm on the warning, the system automatically cancels the open activities when the case is resolved.

### Considerations for case creation automation
>When working with the **Customer Service Hub**, you can access automatic record creation and update rules from the **Service Management** area in Dynamics 365.


> [!important] 
> You can create multiple rules for a single source type, it's important to remember that you can have only one active rule for the same source type and queue at any time.
The same thing occurs if you have two rules that aren't associated with any specific queue but that have the same source type. Be aware of this behavior as you design rules.

### Case management scenarios
![[Pasted image 20240829173238.png]]

### Case management dashboard scenarios
There are two types of interactive dashboards available:
- **Multi-Stream Dashboard (Tier 1)** A multi-stream dashboard displays data in real time over multiple data streams. The data in a stream is based on an entity’s view or a queue, such as My Activities, My Cases, or Cases in the Banking Queue. While a stream always contains information only about one entity, each stream on the dashboard may contain information about a different entity. 
![[Pasted image 20240829173933.png]]
- **Single-Stream Dashboard (Tier 2)** Single-stream dashboards display real-time data over one stream based on a view or queue, for example Active Cases. All the charts on the dashboard are associated with the data stream. Additionally, a single-stream dashboard contains tiles. The tiles are positioned on the right side of the dashboard and are always shown. Single-stream dashboards are useful to users who need to monitor fewer, but more complex or escalated cases in a single view or queue. Out of the box Customer Service hub contains a single-stream.
![[Pasted image 20240829174054.png]]

>Another feature of the Customer Service Hub is the ability to work with entity specific dashboards. Entity specific dashboards are just what the name describes; there are multi-stream dashboards that display data streams related to a single entity such as cases.

### Case management work with cases scenarios
![[Pasted image 20240829174241.png]]

![[Pasted image 20240829174455.png]]
> [!NOTE]
Only one option can be defined per organization.
**None:** Closing the parent case has no effect on child cases. Child cases must be closed individually.
**Close all child cases when parent is closed:** Any open child cases are automatically closed when the parent case is closed. 
**Don't allow parent case closure until all child cases are closed:** All child cases must be closed before the parent case can be closed.

### Use Copilot to assist in resolving customer issues
With Copilot, you can take the following actions:
- **Ask a direct question**: Copilot shows the most relevant answer from the knowledge sources your organization has made available.
- **Ask follow-up turn by turn questions**: If Copilot's response isn't immediately useful, you can ask follow-up questions and guide Copilot in a natural, conversational way.
- **Ask Copilot to attempt a better response**: Copilot can also rephrase responses based on more guidance such as, "Can you summarize your response?" or "Can you attempt a response providing details for each of the steps you mentioned?"

### Work with status reason transitions
Out of the box, specific statuses are available for each Dynamics 365 record, depending on the type of record. Cases have three statuses that they can be in:
- **Active:** The case is currently open and is actively being worked on in the application.
- **Resolved:** The issue for the case has been fixed.
- **Canceled:** The case is no longer active in the system, but it wasn't resolved.

Each record type has what's called a _status reason_. A status reason is associated with a specific record status and provides more information about why the record is in that status. For cases in Dynamics 365, several status reasons are available out of the box:
- **Active:**
    - **In Progress**: The case is currently being worked on by a customer service agent.
    - **On Hold**: The case is active, but it isn't currently being worked on.
    - **Waiting for Details**: The case is active, but you're waiting for more information from the customer.
    - **Researching**: The case is currently being researched.
- **Resolved:**
    - **Problem Solved**: A successful resolution was found for the case.
    - **Information Provided**: The customer was given satisfactory information, and the issue was fixed.
- **Canceled:**
    - **Canceled**: The case was canceled.
    - **Merged**: The case was canceled because it was merged with another record.
> [!tip] 
> You can add, remove, or change case status reasons as needed by going to **Customizations** > **Cases** > **Fields** and selecting the drop-down arrow in the **Status Reason** field. Multiple status reasons are available for each status, and they can be changed.

![[Pasted image 20240829180346.png]]

## Use queues to manage case workloads
[(More)](https://learn.microsoft.com/en-us/training/modules/using-dynamics-365-queues-to-manage-case-workloads/)
### Introduction
Several types of queues are available in Dynamics 365:
- **Public:** These queues are visible to the whole organization.
- **Private:** The queues are visible only to users who have been designated as queue members.
- **Personal:** These queues are associated with a specific user or team, and are visible only to that user or team.

### Configure tables for queues
>Using the navigation on the left, expand **Dataverse** and select **Tables**. Open the table that you want to enable for queues. Once the table is open, select **Properties**. In the **Properties** menu on the right, expand **Advanced** options. Under the **Rows in this table** section, select **Can be added to a queue**.


### Create a Microsoft Dynamics 365 queue
>Queues can be created in the **Customer Service admin center** application. To create queues, select the **Queues** option under **Customer support**, then select **Manage** next to **Basic Queues**.

In addition to specifying a mailbox record for a queue, you can define which emails that come into the queue will be converted to email activities. You have several options:
- All email messages
- Email messages in response to Dynamics 365 email
- Email messages from Dynamics 365 leads, accounts, or contacts
- Email messages from Dynamics 365 records that are email enabled

> [!important] 
> Before a queue can receive email, the mailbox that's associated with the queue must be approved and turned on. In this way, you indicate that it's OK for the mailbox to receive email, and that it's ready to do so. Select the **Open Mailbox** button on the command bar, select **Approve Mailbox**, and then select the **Test and Enable** button.

### Queue items
> [!hint] 
> Basically, there's a one-to-one relationship between the queue item and the record that it's associated with

![[Pasted image 20240829185949.png]]
Queue items can be _removed_ from a queue at any time by users who have sufficient security permissions. When an agent removes a queue item from a queue, the associated record (for example, a case) isn't affected. Only the queue item is removed. ==Don't confuse the remove with the delete action.==
- **Remove:** This action just removes the queue item from the queue.
- **Delete:** This action removes the queue item from the queue **and** deletes the original record (for example, a case).

**Releasing** a queue item from a queue removes the name of the person who's currently working on the queue item record.

### Routing rule sets
- **Basic routing**: Typically used to route records such as cases, leads, emails, etc. to individuals, teams, or queues based of different rule criteria defined. The criteria used with the basic routing feature is typically basic and simple.
- **Unified Routing (Advanced Routing)**: Provides more advanced routing capabilities that directs incoming work to the best-suited queue and agent. Unified routing provides more advanced routing capabilities.

## Agent collaboration in Customer Service
[(More)](https://learn.microsoft.com/en-us/training/modules/agent-collaboration/)
### Introduction
Dynamics 365 Customer Service provides multiple options for agents to collaborate:
- **Embedded chat by using Teams** - Agents can start a new chat or link an existing chat to a record in Teams without switching context or leaving the application. Linking all associated chats to a record can help agents maintain the chats in one place.
- **Customer support swarming by using Teams** - Helps agents quickly resolve issues by bringing together the right experts across your business.
- **Sharing Dynamics 365 records within Microsoft Teams** - Agents can share the record of the chat conversation and let participants view it without navigating away from Teams.

### Set up Microsoft Teams chat
Several standard record types, including case, account, contacts, knowledge article, and email, are available out-of-the-box, or you can add your desired record type. To add more record types, select the **Add Record Types** option and then specify the record type that you want to add.
Within the record type, you can specify the following parameters:
- **Link Chat**
    - **Join chat** - When this feature is turned on, collaborators with correct permissions can join linked chats.
    - **Auto-naming** - This option will name chats with the name of the record that the chat is linked to. If this option is turned off, collaborator's names will be used as the chat name.
- **Unlink chats**
    - **Record owner can unlink** - Specifies that the record owner can unlink any chats.
    - **Recent chat linker can unlink** - Specifies that the person who initially linked the chat to the record can unlink chats.
- **Provide context for new linked chats** - If the **Introduction message** toggle is turned on, when someone starts the chat, they can send information that's related to the linked record to give collaborators context.
- **Suggest contacts** - When the **Rules-based suggested contacts** toggle is turned on, you can set up rules to determine how to suggest contacts that are related to the record.

### Use embedded Teams chat in Customer Service
![[Pasted image 20240829211800.png]]
The preceding image shows what the user experience looks like and a breakdown of the different elements that are part of the embedded chat functionality (as described in the corresponding numbered list).
1. **New chat** - Create chats that aren't associated with Dynamics 365 records.
2. **Filter** - Filter chats by name.
3. **Chats linked to other records** - Chats that are associated with other Dynamics 365 records that the current user is part of. Users can prioritize responses to these chats over other chats.
4. **New linked chat** - Start a new chat that's linked with the record. Only chat participants can view these chats in Dynamics 365.
5. **Other chats** - Chats that aren't linked to records or started from Teams.
6. **Chat control** - Allows users to multitask across chats.
7. **Basic Teams functions** - Format, use emojis, use GIFs, set delivery options, and attach files.
8. **Add/remove participants** - Select who participates in the chat and who doesn't.

When starting a conversation, you can use one of the following approaches:
- **Start a new linked chat with a participant** - Select **New linked chat**. In the **Linked to this record section**, enter the name(s) of the participant(s) whom you want to chat with.
- **Start a chat with a suggested contact** - If an administrator has set up the suggested contacts features, you can select the contact from the suggested contact list and then select **Start a linked chat**.

### Microsoft Teams meeting integration
To ensure that the feature will work correctly, you'll need to set up the following functionality:
- **Sync calendars** - This optional setting ensures that the meetings that are created in Dynamics 365 are added to Microsoft Outlook and Teams and that they appear on agent calendars. For more information, see [Set up server-side synchronization of email, appointments, contacts, and tasks](https://learn.microsoft.com/en-us/power-platform/admin/set-up-server-side-synchronization-of-email-appointments-contacts-and-tasks/).
- **Add and join meetings** - This required setting ensures that an agent can create and join Microsoft Teams meetings directly from Dynamics 365. For more information, see [Manage feature settings](https://learn.microsoft.com/en-us/power-platform/admin/settings-features/).

As an agent, you can:
- Create and join Microsoft Teams meetings directly from Dynamics 365.
- Access and update Dynamics 365 records seamlessly within the context of a Microsoft Teams meeting.
- Capture notes and tasks seamlessly during a Microsoft Teams meeting, and have these notes and tasks automatically sync to records in Dynamics 365.

#### Meeting life cycle
You can divide the life cycle of a meeting into the following stages, with each stage catering to specific tasks:
- **Pre-meeting** - In this stage, you'll need to perform the following tasks:
    - [Create a Teams meeting](https://learn.microsoft.com/en-us/dynamics365/customer-service/use-teams-meetings#create-a-teams-meeting).
    - [Join a Teams meeting](https://learn.microsoft.com/en-us/dynamics365/customer-service/use-teams-meetings#join-a-teams-meeting).
    - [Add Dynamics 365 app to a Teams meeting](https://learn.microsoft.com/en-us/dynamics365/customer-service/use-teams-meetings#add-dynamics-365-app-to-a-teams-meeting).
    - [Use the Dynamics 365 app to view and update record information](https://learn.microsoft.com/en-us/dynamics365/customer-service/use-teams-meetings#work-with-the-dynamics-365-app).
- **In-meeting** - In this stage, you'll need to perform the following tasks:
    - Use the side panel to view and update record information.
    - [Work with notes during a meeting](https://learn.microsoft.com/en-us/dynamics365/customer-service/use-teams-meetings#work-with-notes-during-a-meeting).
    - [Work with tasks during a meeting](https://learn.microsoft.com/en-us/dynamics365/customer-service/use-teams-meetings#work-with-tasks-during-a-meeting).
    - [Work with activities during a meeting](https://learn.microsoft.com/en-us/dynamics365/customer-service/use-teams-meetings#work-with-activities-during-a-meeting).
- **Post-meeting** - In this stage, you need to [use the Dynamics 365 app to view and update record information](https://learn.microsoft.com/en-us/dynamics365/customer-service/use-teams-meetings#work-with-the-dynamics-365-app).

### Set up customer support swarming for complex cases
>Customer support swarming is a collaborative approach to solving customer issues. It allows you to bring together experts across your entire business to help agents solve issues. For example, while working on an ongoing Internet of Things (IoT) related issue, an agent might require assistance from an IoT engineer who has knowledge of the device and how it integrates with a specific piece of routing equipment. The agent might also require assistance from an engineer who's familiar with the routing equipment. Additionally, they need to engage with someone in operations to solve a logistical issue with the device.

The **Customer support swarming** page is where you can set up the different elements that will be applied as part of case swarming. You can access the **Customer support swarming** page from the Customer Service admin center. Under **Agent experience**, select **Collaboration** and then select **Customer Support Swarming**.
![[Pasted image 20240830003534.png]]
The preceding image shows the various components of the **Customer support swarming** page (corresponding with the following numbered list):
1. **Swarming toggle** - Turns on the swarming feature.
2. **Agent swarm guide** - Administrator-provided guidance to help agents know what content to include to begin a swarm or manage the swarm process.
3. **Case details** - Add out-of-the-box case fields. Administrators can set up which case fields will show on the form.
4. **Skills** - Add relevant skills to help match experts for swarming. Add coworkers who are outside of your team as experts (through mapping or bulk-importing) so that they can be recommended for swarms.
5. **Rules for skills** - Conditions that define which skills to attach to swarms. The attached skills will be used to find and invite experts to swarms.
6. **Participants automatically added to swarms** - Team contacts are automatically added to swarms because of their relationship to the customer or the agent who's assigned to the issue.
7. **Swarm expert notification** - The Power Automate flow that turns on and manages swarm invitations that are sent to experts.

>If your organization is already using skills, you can reuse them to define swarm rules. You can define skills from the **Customer support swarming** page, but you'll need to select **Go to skill** in the skill section. When defining a skill/characteristic, you'll specify the following details:
>  - **Name** - Defines the name of the skill or certification as it will be presented in the application.
>  - **Description** - A short description that will provide more details about the skill.
>  - **Characteristic type** - Specifies whether this item should be classified as a skill or a certification.

>As mentioned previously, swarming uses bookable resource records to identify experts who will be able to assist with the item. If your organization is already using bookable resources in resource scheduling or with Omnichannel for Customer Service, you can reuse the resources to define your swarm rules. If you haven't already set up experts, you can do so in the Customer Service admin center. Under the **Operations** group, select **Service scheduling** and then select **Manage** next to **Resources**.

### Use customer support swarming
>When an agent is working with a customer and needs to engage with subject matter experts, they can initiate a swarm request. They can do so by selecting the **Create swarm** button on the command bar.

On the **Swarm** page, enter information into the following fields:
- **Swarm request** - Question or statement that reflects what you want help with. The question or statement, such as "coffee machine is broken," will be used to find skills and experts to help you.
- **Steps already tried** - Provide details about steps that you've already taken to try to resolve the issue and any results. These details help confirm that required processes have been followed, and it also provides immediate context for other swarm participants who are invited to collaborate on the issue.
- **What skills do you need?** - The system will attempt to match skills based on your swarm question. The suggested skills are based on the case title and any other case-related conditions that were defined as swarm condition rules. Suggested skills have the light bulb icon next to them. You can also manually select skills that you think are relevant to the case. You can select up to 10 skills (system suggested and manually selected.)

When you select an expert for your swarm, they'll be sent an automated invitation through an adaptive card. When they accept your invitation, they're attached to the swarm and their skills will be indicated. If the expert declines the invitation, the system will look for the next expert(s) that have the needed skill(s).
The **swarm invitation** shows the following information:
- **Inviting agent** - The agent who initiated the swarm and invited the expert.
- **Swarm request** - The question that the agent needs help with.
- **What the agent has tried** - A brief description of what the agent has tried prior to creating the swarm.
- **Expert skills** - The required skills that the expert has for the swarm.
- **Accept and reject** - Options for the expert to join or decline the swarm. If an expert declines an invitation and then later decides that they want to join, they can participate by asking you to add them manually. They won't be able to view the **Swarm** page from the group chat.

## Create or update records automatically in Customer Service Hub
[(More)](https://learn.microsoft.com/en-us/training/modules/auto-create-records-hub/)
### Introduction
A typical update and creation rule must include the following three items:
- **Activity type to monitor** - Defines which of the available activity types in the organization that the creation and update rule applies to.
- **Conditions to evaluate** - Defines what criteria the record must meet to be converted to a case. For example, you might specify that the email activity must come from a gold-level support customer.
- **Actions to take** - Defines what actions that the rule should take when the condition is met. For example, if the email is from a gold-level customer, create a new case record and associate it with the customer from whom the email was received.

### Set up rules to create or update records automatically
When you create a rule, you first need to define the following information:
- **Rule name** - Defines the name of the rule.
- **Queue to monitor** - Specifies which queue (if any) that the rule monitors to look for records. For example, you might specify monitoring your organization's default support queue.
- **Activity type to monitor** - Specifies which type of activity record that the rule looks for when applying the rule.

> [!important] 
> For an email source type, specifying a queue is mandatory. For all other source types, including custom activities, it's optional.

### Configure rules for creating or updating records automatically
>Rule items define the conditions to evaluate and the actions to take based on the conditions. Likely, a single rule has multiple rule items defined for it. As the rule is applied to an incoming record, each rule item is evaluated in the order that is defined in the rule.

>Conditions can evaluate specific contents in the activity to convert to a Dynamics 365 record or from records that are related to it. For example, you can define a condition that looks at the account or contact record that is associated with the sender of the email.

After you define the conditions to evaluate, you need to specify the action to take when the condition is met, such as creating a case record. The two main parts to actions are:
- **Record to create** - Specifies which type of record that the rule creates.
- **Configure in Microsoft Power Automate** - Uses Microsoft Power Automate to define the specific details of the record to create.

### Map records manually with Power Automate
When you select **Save and open Power Automate**, a Power Automate flow opens on a new tab. The flow needs to connect to the Microsoft Dataverse connector to populate data, so you might need to sign in to the connector. After you sign in, the flow will appear.

Initially, the flow includes five items:
- **When the incoming activity triggers the flow** - The flow triggers based on information that is coming from Dynamics 365.
- **Identify email sender** - Captures the name of the person from whom the email came.
- **Is this email sender a contact or an account** - Determines if the email was received from an existing account or contact in the system.
- **Create a record** - Creates the new record in the system.
- **Connect the record to the incoming activity** - Associates the created record with original incoming email activity record.

Three steps where editing or deleting is limited:
- **When the incoming activity triggers the flow** - Don't edit or delete this step.
- **Create a record** - You can modify this step as needed, but make sure that you don't rename or delete it.
- **Connect the record to the incoming activity** - Don't edit or delete this step.
Other than the preceding steps, other steps can be edited, added, or removed to better fit your needs.

The triggering step that defines how the flow is getting triggered is **When the incoming activity triggers the flow**. All information in the step is predefined and based on the activity type that was specified when the rule was created. Two main items that this step specifies:
- **Change type** - Defines what record event triggers the flow. In this case, it's triggered after an email activity that was created in the system is updated, which happens when the rule runs against the item.
- **Table name** - Defines the Microsoft Dataverse table that the activity is associated with. In this case, because the rule is associated with an email activity, it's using the Email Messages table.

### Use the activity monitor to review and track rules
>You can review and track the overall health of your automatic record creation rules and resolve issues around them by using the activity monitor. The activity monitor tracks and evaluates rules while they are being implemented in Customer Service Hub and before the rule is run in Power Automate.

You can access the activity monitor in two different ways:
- From the **Activity monitor** for each individual rule.
- By selecting the **View Activity Monitor** button on the command bar from the **Automatic record creation and update rules** list.

Regardless of the method that you select, the following details are available for the rules:
- **Current state** - Displays the state of the rule. Three primary outcomes will display:
    - **Failed** - Identifies that the system tried to run the rule, but it failed for some reason.
    - **Skipped** - Identifies that the system didn't attempt to run the rule on the record for some reason. For example, the sender doesn't have an entitlement record associated with them.
    - **Ready for Power Automate** - Indicates that the system processed the rule on the Customer Service end and that it's ready for Power Automate to take over.
- **Rule name** - Defines the name of the record creation rule that was monitored.
- **Monitored activity type** - Defines the activity type that the rule was associated with such as email, task, or appointment.
- **Monitored activity item** - Displays the subject of the activity type.
- **Condition name** - Identifies the name of the condition where the issue was found.
- **Reason** - Displays information on how the rule was handled.
    For example, if the value in **Current state** for a rule is **Skipped**, no action was taken because, on the **Advanced** tab of the rule, a rule condition such as **Allow emails from unknown senders** was set to **No**. Therefore, if the email was from an unknown sender, no further action was required.
- **Evaluated on** - Displays the date and time of the issue.
![[Pasted image 20240830012055.png]]

