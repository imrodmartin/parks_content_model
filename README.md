# Parks Content Model

A Drupal recipe with the Parks & Recreation content model that trainees build by hand in Learning Module 2 of the Drupal 12 Site Building course:

- Content types: **Program** (`program`) and **Facility** (`facility`), with titles relabeled *Program name* and *Facility name*
- Program fields: `field_summary`, `field_description`, `field_image`, `field_facility`, `field_activity_type`, `field_age_group` (unlimited), `field_season`, `field_session_dates`
- Facility fields: `field_address`, `field_hours`, `field_accessibility`, `field_image` (shared storage with Program)
- Vocabularies: **Activity type** (`activity_type`), **Age group** (`age_group`), **Season** (`season`)
- Form and view displays, including the Program **Teaser** display
- Core's `image_media_type` recipe, which `field_image` depends on

It holds structure only: no terms, no content. Use `parks_demo_content` for those.

## Who runs it

Trainees don't apply it directly. The Layout and Theming course's `parks_theming_setup` recipe applies it, so a trainee who skipped Site Building gets the same model. It uses `strict: false`, so on a site where the model already exists nothing is changed.

The config was taken from a finished Site Building site, with the parts later modules add (Layout Builder, Content Moderation, Redirect) removed.
