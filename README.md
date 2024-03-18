# Fork of Open Y Activity Finder

## Motivation
We had a lot of customizations for the YGBW site, and all customization was stored as local patches.
It's become hard to manage, so we decided to move these changes to separate fork

## Versions
We use 4.2.7 version of the ycloudyusa/yusaopeny_activity_finder module. 
These patches were applied to customize AF:

```json
 "ycloudyusa/yusaopeny_activity_finder": {
                "Fix SolrBackend errors": "./patches/openy_activity_finder/ActivityFinder_Fix_SolrBackend_errors.patch",
                "Fix max age period to match ActiveNet with less than value": "./patches/openy_activity_finder/activity_finder_max_age_fix.patch",
                "Add week display to min age": "./patches/openy_activity_finder/activity_finder_min_age_week_display.patch",
                "Hide camp and facility filters": "./patches/openy_activity_finder/hide_camp_and_facility_filter.patch",
                "Fix prices display": "./patches/openy_activity_finder/fix_prices_display.patch",
                "Add AF text field to activity details modal": "./patches/openy_activity_finder/af_text_field.patch",
                "Added custom learn more link": "./patches/openy_activity_finder/learn_more.patch",
                "Add availability note": "./patches/openy_activity_finder/availability_note.patch",
                "YGBW Ads": "./patches/openy_activity_finder/ads.patch",
                "Allow links in the class description": "./patches/openy_activity_finder/af_allow_links_in_class_description.patch",
                "YGBWSLA-495 - SEO parameters": "./patches/openy_activity_finder/ygbwsla-495-seo-parameters.patch",
                "YGBWSLA-527 (3)": "./patches/openy_activity_finder/add_scroll_to_top_for_update_url.patch",
                "YGBWSLA-532 - Issues with Activity Finder": "./patches/openy_activity_finder/add_checks_for_missing_index_errors.patch",
                "Add months filter": "./patches/openy_activity_finder/add_months_filter.patch",
                "Replace location id by label for SelectLocations step": "./patches/openy_activity_finder/replace_location_id_by_label_for_SelectLocations.patch",
                "Add multiple dates support to AF": "./patches/openy_activity_finder/multiple_dates.patch"
            },
```