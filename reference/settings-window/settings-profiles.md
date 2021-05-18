**Settings**
---

## Alaska Region mdEditor Profiles

![Profile Settings Dashboard](/assets/reference/settings/settings-profile.png)

#### What are mdEditor Profiles?

The mdEditor is designed to support creating metadata for a wide variety of data types. As a result, an edit session will likely display much more information than is required for the data that you are describing. Applying a profile allows a user to hide menus and data entry fields that may not be required for a given use case.

A mdEditor custom profile consists of a "**profile definition**" and an associated "**validation schema**". Multiple validation schemas may be associated with a single profile definition. Each unique combination of a definition and schema is a distinct mdEditor profile.

{% hint style='tip' %}
**Note**: The mdEditor defaults to the **"Full Profile"** when a metadata record is first created, displaying all available menus and data entry fields.
{% endhint %} 

#### What Is a Validation Schema?

A validation schema is a file or set of files that specify the metadata fields that must contain data for a record to be considered valid. The validation schema controls when an error message is displayed by the editor.

#### Creating Profile Definitions and Schemas

A discussion of creating profiles and schemas is beyond the scope of this documentation. Contact your Data Manager or Data Steward for assistance.

#### Editing A Profile Record

When editing a record, a Profile Selection field is displayed on the mdEditor Primary Navigation Bar. A selected profile will remain associated with metadata record unless changed during a subsequent edit session.

#### Adding a custom profile to mdEditorCreating Profile Definitions and Schemas

Before a custom profile can be created for use in the mdEditor, the profile definition and validation schema must be accessible as URLs. 

{% hint style='tip' %}
**Note**: if you are using GitHub to host profile definition files, make sure that you provide users with the URL to the "raw" version of the file.
{% endhint %} 

###### Steps to Add a Profile Definition (Screenshots to be added)

1. Go to Settings/Profiles/Manage Definitions.

2. Select "Add Definition".

3. Select "Imported" tab.

4. Enter URL to profile definition.

5. Enter an optional alias (the alias replaces the definition title).

6. Select "Save definition". You should receive a notification that the profile has been downloaded and profile information will be displayed on the tab.


###### Steps to Add Validation Schema (Screenshots to be added)

1. Go to Settings/Profiles/Validation.

2. Select "Add Schema".

3. Enter URL to the schema root.

4. Enter a Title and Description.

5. Select the record "Type" to which the schema applies.

6. Select "Save Schema". You should receive a notification that the profile has been downloaded.



###### Steps to Add A Profile for Use by mdEditor (Screenshots to be added)

1. Go to Settings/Profiles.

2. Select "Add Profile".

3. Enter a "Title" (displayed in profile selection field). 

    * Select a "Profile Definition" from the drop-down list (either the definition title or the alias entered in the previous step will be displayed). 
    
    * Add optional description (displayed when cursor hovers over "?" in the profile selection field).
 
4. Identify a schema from the "Selected Schema" list and select "Add" (NOTE: Skip this step for testing. You will see a "No schemas have been assigned" warning, just ignore that for now!).

5. Select "Save Profile".


{% hint style='tip' %}
**Note**: Changes made to a existing profile may not be reflected until the editor is reloaded.
{% endhint %} 

###### Steps for Updating a Profile (Screenshots to be added)

1. Go to Settings/Profiles/Manage Definitions

2. Select "Check for Updates"

3. A blue information icon next to a profile definition indicates that an update is available.

4. Select the definition "Edit" button. (The currently installed version will be displayed along with the updated version in a blue box)

5. Select "Update Definition" button to proceed with update.

6. Refresh browser to activate updated profile.

---


##### Currently Available Alaska Region Profile Definitions

**Alaska Region basic project definition (alpha version)**


* File name: ak-proj-a.json
* URL: https://raw.githubusercontent.com/USFWS/ak-md-profiles/main/ak-proj-a.json



**Alaska Region basic product definition (alpha version)**


* File name: ak-prod-a.json
* URL: https://raw.githubusercontent.com/USFWS/ak-md-profiles/main/ak-prod-a.json


---

#### Resources

* Core Profile Definitions for the mdEditor: https://adiwg.github.io/mdProfiles/

* Core Schema: https://raw.githubusercontent.com/adiwg/mdJson-schemas/master/schema/schema.json

* ADIwg mdProfiles: https://github.com/adiwg/mdProfiles

* mdJson-schemas: https://github.com/adiwg/mdJson-schemas

---

