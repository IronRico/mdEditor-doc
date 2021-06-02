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

###### Steps to Add a Profile Definition 

1. From the Profiles tab, Select Manage Definitions.

![Adding Profile Definition Step 1](/assets/reference/settings/profileImages/ProfileDefStep1.png)

2. Select "Add Definition".

![Adding Profile Definition Step 2](/assets/reference/settings/profileImages/ProfileDefStep2.png)

3. Select "Imported" tab.

![Adding Profile Definition Step 3](/assets/reference/settings/profileImages/ProfileDefStep3.png)

4. Enter URL to profile definition.

![Adding Profile Definition Step 4](/assets/reference/settings/profileImages/ProfileDefStep4.png)

5. Enter an optional alias (the alias replaces the definition title).

![Adding Profile Definition Step 5](/assets/reference/settings/profileImages/ProfileDefStep5.png)

6. Select "Save definition". You should receive a notification that the profile has been downloaded and profile information will be displayed on the tab.

![Adding Profile Definition Step 6](/assets/reference/settings/profileImages/ProfileDefStep6.png)


###### Steps to Add Validation Schema 

1. Go to Settings/Profiles/Validation.

![Add A Validation Schema Step 1](/assets/reference/settings/profileImages/AddValidation1.png)

2. Select "Add Schema".

![Add A Validation Schema Step 2](/assets/reference/settings/profileImages/AddValidation2.png)

3. Enter URL to the schema root.

![Add A Validation Schema Step 3](/assets/reference/settings/profileImages/AddValidation3.png)

4. Enter a Title and Description.

![Add A Validation Schema Step 4](/assets/reference/settings/profileImages/AddValidation4.png)

5. Select the record "Type" to which the schema applies.

![Add A Validation Schema Step 5](/assets/reference/settings/profileImages/AddValidation5.png)

6. Select "Save Schema". You should receive a notification that the profile has been downloaded.

![Add A Validation Schema Step 6](/assets/reference/settings/profileImages/AddValidation6.png)



###### Steps to Add A Profile for Use by mdEditor 

1. Go to Settings/Profiles.

![Add A New Profile Step 1](/assets/reference/settings/profileImages/AddProfileStep1.png)

2. Select "Add Profile".

![Add A New Profile Step 2](/assets/reference/settings/profileImages/AddProfileStep2.png)

3. Enter a "Title" (displayed in profile selection field). 

    * Select a "Profile Definition" from the drop-down list (either the definition title or the alias entered in the previous step will be displayed). 
    
    * Add optional description (displayed when cursor hovers over "?" in the profile selection field).
        
 
4. Identify a schema from the "Selected Schema" list and select "Add" (NOTE: Skip this step for testing. You will see a "No schemas have been assigned" warning, just ignore that for now!).


5. Select "Save Profile".

![Add A New Profile Step 3-5](/assets/reference/settings/profileImages/AddProfileStep3-5.png)

6. Check to see if the new profile appears in the profile list.

![Add A New Profile Step 6](/assets/reference/settings/profileImages/AddProfileStep6.png)

{% hint style='tip' %}
**Note**: Changes made to a existing profile may not be reflected until the editor is reloaded.
{% endhint %} 

###### Steps for Updating a Profile 

1. Go to Settings/Profiles/Manage Definitions

![Updating A Profile Step 1](/assets/reference/settings/profileImages/UpdatingAProfile1.png)

2. Select "Check for Updates"

![Updating A Profile Step 2](/assets/reference/settings/profileImages/UpdatingAProfile2.png)

3. A blue information icon next to a profile definition indicates that an update is available.

![Updating A Profile Step 3](/assets/reference/settings/profileImages/UpdatingAProfile3.png)

4. Select the definition "Edit" button. (The currently installed version will be displayed along with the updated version in a blue box)

![Updating A Profile Step 4](/assets/reference/settings/profileImages/UpdatingAProfile4.png)

5. Select "Update Definition" button to proceed with update.

![Updating A Profile Step 5](/assets/reference/settings/profileImages/UpdatingAProfile5.png)

6. Refresh browser to activate updated profile.

![Updating A Profile Step 6](/assets/reference/settings/profileImages/UpdatingAProfile6.png)

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

