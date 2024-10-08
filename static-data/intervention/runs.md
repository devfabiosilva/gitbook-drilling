# Runs

{% hint style="info" %}
From the plugin-wells 2.28.0 it is possible to represent runs in a section
{% endhint %}

### New section data representation

![](<../../.gitbook/assets/image (45).png>)

Geometry data remains at the same level - one per section

![](<../../.gitbook/assets/image (195).png>)

Run data changes depending on the type (Drilling or Casing)

![](<../../.gitbook/assets/image (496).png>)

### Creating a run

In a section, click on “add run” and choose between “Drilling” or “Casing”

![](<../../.gitbook/assets/image (106).png>)

### View section details

Click on the section details area

![](<../../.gitbook/assets/image (41).png>)

### Migration of section data to runs

When the plugin-well upgrades to version 2.28.0, the old section data is represented within a run. This run will have a flag indicating that data has been migrated from the section.

![](<../../.gitbook/assets/image (386).png>)
