Duplicate checking
==================

openEQUELLA 2019.2 sees the introduction of attachment duplicate checking, as
well as enhancements to the existing edit box duplicate checking functionality.

Configuring duplicate checking
------------------------------

Duplicate checking is configured from the attachment or edit box wizard control
in the Collection Definition Editor, accessed from the Administration Console.

### Attachments

Attachment duplicate checking allows administrators to notify contributors of
existing items that have the same attachments. This includes *Files* and *URL
Links* attachment types. For example, if duplicate checking is enabled for
‘Files’ in an attachment control in a contribution wizard, the contributor sees
a **Duplicate warning** message if a file a contributor uploads is an exact
match to a file that has been uploaded in one or more existing items in the same
collection. A link is provided to those items so they can be viewed before
proceeding.

The duplicate checking for attachments is switched on in the configuration
sections for *Files* and *URL Links* attachment types.

##### To enable File duplicate checking

1.  From the **Administration Console**, select **Collection Definitions**. An
    example is shown in Figure 1

   ![](073690b9817231fc53b3a84243a2bc8b.png)

   Figure 1 Administration Console - Collection Definitions

2.  Double click the collection containing the relevant attachment control (or
    highlight and select **Edit)**.

3.  From the **Wizard** tab, select the attachment control with the *Files*
    attachment type that requires duplicate checking to be applied.

4.  Scroll to the **Files** configuration section and check **Enable duplicate
    checking.** An example is shown in Figure 2.

   ![](2c1acfdd4388b5c76a2f5317160c2d69.png)

Figure 2 Attachment control – Files configuration

5.  Click **Save.**

##### To enable URL duplicate checking

1.  From the **Administration Console**, select **Collection Definitions**. An
    example is shown in Figure 3.

   ![](073690b9817231fc53b3a84243a2bc8b.png)

   Figure 3 Administration Console - Collection Definitions

2.  Double click the collection containing the relevant attachment control (or
    highlight and select **Edit)**.

3.  From the **Wizard** tab, select the attachment control with the *URL Links*
    attachment type that requires duplicate checking to be applied.

4.  Scroll to the **URL Links** configuration section and check **Enable
    duplicate checking.** An example is shown in Figure 4.

   ![](d953b93a1cce8d937d00457cc97ddc22.png)

   Figure 4 File attachment control – URL Links configuration


5.  Click **Save.**

### Edit boxes

Duplicate checking for edit boxes allows administrators to notify contributors
of existing items that contain the exact text string entered in the same edit
box field. For example, if duplicate checking is enabled for the ‘Title’ edit
box in a contribution wizard, the contributor sees a **Duplicate warning**
message if the text they have entered for the title is an exact match to the
text in the ‘Title’ field for one or more existing items in the same collection.
A link is provided to those items so they can be viewed before proceeding.

Duplicate checking can be switched on for multiple edit box wizard control in
one collection. For example, duplicate checking could be enabled for both the
‘Title’ and ‘Description’ fields in one contribution wizard. Any text entered in
the ‘Title’ field would be matched against existing item titles within the
collection, and any text entered in the ‘Description’ field matched against
existing item descriptions within the collection.

##### To enable Edit box duplicate checking

1.  From the **Administration Console**, select **Collection Definitions**. An
    example is shown in Figure 5.

   ![](073690b9817231fc53b3a84243a2bc8b.png)

   Figure 5 Administration Console - Collection Definitions

2.  Double click the collection containing the relevant edit box (or highlight
    and select **Edit)**.

3.  From the **Wizard** tab, select the edit box that requires duplicate
    checking to be applied.

4.  Select **Warn contributor if data in this field is not unique for resources
    in this collection.** An example is shown in Figure 6.

   ![](e3554c57501257ab68ac24a0482d7184.png)

   Figure 6 Collection Definition Editor - Wizard tab

5.  Click **Save.**

Duplicate checking during contribution
--------------------------------------

Duplicate checking occurs during the contribution and editing of items.

### Attachment duplicate checking

A duplicate warning message displays as soon as a file has completed uploading
or a URL Link is added if an exact match is identified in one or more items in
the same collection.

NOTE: File duplicate checking works using MD5 hashes, so the same files with
different names are still identified as duplicates if uploaded.

NOTE: Attachment duplicate checking does not search for matches in items with
the status of Deleted, Suspended, Archived or Rejected.

An example is shown in Figure 7.

![](df16a9316d225580aed2d34bd931c616.png)

Figure 7 File duplicate warning

Click on the **Click here to view existing items that contain duplicates** link
to open the **Duplicate data** page. A list of items containing matching text
displays. An example is shown in Figure 8.

![](ce1798d3dfc9d8cde030baf0e060e236.png)

Figure 8 Duplicate data page

Note that the contributor can choose to ignore the duplicate warning and save
the item without opening the link. The Duplicate data page can still be viewed
when editing the item.

Click on the item links to open the items in new tabs.

The **Duplicate data** page can also be accessed from the pages box and using
the navigation button.

![](cdd366d5a499d233bdae4d55d9147d5b.png)

Figure 9 Navigating to Duplicate data page

### Edit box duplicate checking

A duplicate warning displays as soon as the focus moves from the edit box when
an exact match is identified in one or more items in the same collection. An
example is shown in Figure 10.

![](41fcafeb04a0da69a4ebcb89eb233967.png)

Figure 10 Edit box duplicate warning

Note that the contributor can choose to ignore the duplicate warning and save
the item without opening the link. The Duplicate data page can still be viewed
when editing the item.

Click on the **Click here to view existing items that contain duplicates** link
to open the **Duplicate data** page. A list of items containing matching text
displays. An example is shown in Figure 11.

![](03b17822d3516311530c303a20218aff.png)

Figure 11 Duplicate data page

Click on the item links to open the items in new tabs.

The **Duplicate data** page can also be accessed from the pages box and using
the navigation button. An example is shown in Figure 12.

![](181b7229e5fbef2a8a65f3e4345b6932.png)

Figure 12 Navigating to Duplicate data page

### Multiple duplicate types

In the case of the detection of multiple duplicates across edit boxes and
attachment controls during contribution, openEQUELLA shows multiple duplicate
warnings. An example is shown in Figure 13.

![](abb98dd54af719e0be2db00931963091.png)

Figure 13 Item contribution with multiple duplicate warnings

The **Duplicate data** page displays the duplicate items for each wizard control
separately. Additionally, for multiple attachment duplicates, each attachment is
listed separately. An example is shown in Figure 14.

![](2a5903d948bcdad239e40ee3ed3e6be4.png)

Figure 14 Duplicate data page with multiple duplicate lists

Displaying deleted user names
-----------------------------

openEQUELLA 2019.2 now stores owner details in the database so that if a user is
deleted, past ownership and moderation information are not lost.

NOTE: Users must log in to openEQUELLA at least once prior to their deletion for
this functionality to apply.

When a user is removed from openEQUELLA, the system will now display the deleted
user’s name with the word ‘*removed’* in brackets e.g. *Joe Bloggs (removed)*
instead of ‘Unknown user’ in the Owner field, the Moderation history page and
the Owners and collaborators page. This applies to both local openEQUELLA users
and users managed by integrated external user management systems such as LDAP.

An example of the Resource summary page for an item with a deleted owner is
shown in Figure 15.

![](1d3387b927789878c8470e52cb32e676.png)

Figure 15 Owner field with deleted user's details

An example of the Moderation history page (accessed from Details, Moderation
History) with a deleted user’s details is shown in Figure 16.

![](3cb1f7f4cdd8ad1486d96d4f06c9ea60.png)

Figure 16 Moderation history page with deleted user details

NOTE: If an item has been through a workflow process, the details of any
workflow task moderators that have been removed from the system display on this
page.

An example of the Owner and collaborators page (accessed from Actions, Change
ownership) is shown in Figure 17.

![](740d92deb34869c4199f275dc69111ed.png)

Figure 17 Owners and collaborators page with deleted user details

### Filtering items with deleted owners

The existing **Show items with not owner** filtering option accessed from the
**Filter** panel on the Manage Resources page can be used to view only items
that have a deleted user recorded as the owner. It will also return any records
that have the original ‘Unknown user’ label displaying for users that were
deleted prior to the openEQUELLA 2019.2 update.

An example is shown in Figure 18.

![](1d606d1e5ed129fdc75b69b1d5d0a3e2.png)

Figure 18 Manage resources - Show items with no owner filter option

Taxonomy term sorting
=====================

A new option has been added to the Taxonomy editor, Terms page to allow taxonomy
terms to be sorted alphabetically across the whole taxonomy or the child terms
for a selected taxonomy level.

##### To sort child taxonomy terms

1.  From the **Administration Console**, select **Taxonomies**. An example is
    shown in Figure 19.

   ![](1498fbb4f763ccfcacb33d1c72024ba4.png)

   Figure 19 Administration Console - Taxonomies

2.  Double click the taxonomy to be sorted (or highlight and select **Edit)**.

3.  From the **Terms** tab, right click on a taxonomy level to sort the child
    terms for that level then select **Sort Child Terms**. An example before
    sorting is shown in Figure 20.

![](70c827b2f650d9a79f6357cd856064fc.png)

Figure 20 Selected taxonomy level

An example of the right-click menu with the sorting option in shown in Figure
21.

![](86a24bc6d7d472855b32930c00b4e9df.png)

Figure 21 Right-click menu - Sort Child Terms

An example after the terms have been sorted is shown in Figure 22.

![](470c3a034f39c27856d73ccff9ac132a.png)

Figure 22 Sorted child terms

##### To sort across the whole taxonomy

1.  From the **Administration Console**, select **Taxonomies**. An example is
    shown in Figure 23.

   ![](1498fbb4f763ccfcacb33d1c72024ba4.png)

   Figure 23 Administration Console - Taxonomies

2.  Double click the taxonomy to be sorted (or highlight and select **Edit)**.

3.  From the **Terms** tab, right click on any taxonomy level then select **Sort
    Whole Taxonomy**. An example before sorting is shown in Figure 24.

![](601436ed4ab5a67b73daca67c9eb2a67.png)

Figure 24 Sort Whole Taxonomy menu option

An example of the right-click menu with the sorting option in shown in Figure
25.

![](06ec65b26590fb9ef6eff6562fb3ea64.png)

Figure 25 Right-click menu - Sort Whole Taxonomy

NOTE: Every level of taxonomy is sorted alphabetically.

An example after the terms have been sorted is shown in Figure 26.

![](47e9d5e08186240580a15e91d9f6ef46.png)

Figure 26 Sorted taxonomy


