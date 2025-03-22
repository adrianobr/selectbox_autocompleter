# Redmine Selectbox Autocompleter Plugin

This plugin generates autocomplete box for select box.
For example, it is useful for assisting input of a select box containing many option elements.

![ss_author_select2](/docs/ss_author_select2.png?raw=true)


## Installation

```
$ cd $(REDMINE_HOME)/plugin
$ git clone https://github.com/adrianobr/selectbox_autocompleter.git selectbox_autocompleter
```

and restart your redmine.

## Configuration

![configure_default](/docs/configure_default.png?raw=true)

You can configure target (html id attiribute) for convert selectbox to autocomplete box.

Default target list are below.

```
project_parent_id
project_default_version_id
project_default_assigned_to_id
group_id
group_by
operators_user_id
operators_spent_on
operators_status_id
operators_assigned_to_id
operators_author_id
operators_relates
operators_tracker_id
operators_priority_id
operators_fixed_version_id
operators_category_id
operators_done_ratio
operators_is_private
operators_watcher_id
operators_duplicates
operators_copied_to
operators_duplicated
operators_blocked
operators_follows
operators_copied_from
operators_updated_by
operators_last_updated_by
operators_child_id
operators_notes
operators_subject
operators_issue_id
operators_description
operators_tags
operators_any_searchable
operators_created_on
operators_updated_on
operators_closed_on
operators_start_date
operators_parent_id
operators_estimated_hours
operators_spent_time
operators_member_of_group
operators_attachment
operators_attachment_description
operators_assigned_to_role
operators_fixed_version_due_date
operators_due_date
operators_fixed_version_status
operators_precedes
operators_blocks
operators_description
add_filter_select
issue_author_id
issue_project_id
issue_assigned_to_id
issue_tracker_id
issue_status_id
issue_priority_id
issue_assigned_to_id
issue_fixed_version_id
issue_template
issue_done_ratio
values_assigned_to_id_1
values_author_id_1
wiki_page_parent_id
project_quick_jump_box
values_status_id_1
values_tracker_id_1
values_priority_id_1
values_fixed_version_id_1
values_category_id_1
values_watcher_id_1
values_is_private_1
values_tags_1
values_member_of_group_1
values_last_updated_by_1
values_updated_by_1
values_assigned_to_role_1
issue_agile_data_attributes_story_points
user
period
project_id
issue_id
time_entry_activity_id
columns
criterias
time_entry_user_id
month
year
```

### Select2 mode

Convert select box using [Select2](https://select2.github.io/).

![ss_jump_select2](/docs/ss_jump_select2.png?raw=true)

### Datalist mode

Insert input box with datalist.

![ss_jump_datalist](/docs/ss_jump_datalist.png?raw=true)

### jQuery mode

Insert input box with jQuery.  
This is useful for IE and Edge because jQuery list is a partial match; the list by the autocomplete attribute is a forward match in IE and Edge.

![ss_jump_jquery](/docs/ss_jump_jquery.png?raw=true)
