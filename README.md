# Dropshipment-for-SO

Create Drop Shipments from Sales Orders against vendor selected for the lookup custom field

# STEPS

# 1. Create a custom field in the sales order module :

Settings > Preferences > Sales Orders > Field Customization > New Custom Field

Create a Loop-up data type custom field with "Vendor" module as related entity 

# 2. Create Custom function

Settings > Automations > Custom Functions > New Custom Function 

Module: Sales Order

Copy and paste the Dropshipment for SO script.

Create connection for Zoho Inventory - zom

# 4. Create workflow

Settings > Automations > Workflow Rules > New Workflow Rule

Module : Sales Order

Workflow Type : Event Based

When an Sales Order is: Created / Edited

Filter the triggers: When vendor lookup field is not empty 

Choose the appropriate custom function in the Action.

Save the workflow. On each salesorder creation / edit action, the workflow automatically creates a Drop Shipment Purchase Order
