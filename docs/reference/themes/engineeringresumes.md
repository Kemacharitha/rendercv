#let cv = (
  name: "Kema Naga Sai Sri Charitha",
  email: "kemasrimannarayana66@gmail.com",
  phone: "+91 9705912755",
  location: "Bhimavaram, West Godavari, India",

  education: [
    (
      degree: "B.Tech in Artificial Intelligence and Data Science",
      institution: "Sagi Rama Krishnam Raju Engineering College",
      location: "Bhimavaram, India",
      graduation: "2026"
    ),
    (
      degree: "Intermediate",
      institution: "Sri Sai Ram Junior College",
      location: "Ongole, India",
      graduation: "2022"
    ),
    (
      degree: "SSC",
      institution: "R.V.N.Z.P. High School",
      location: "Ravinuthala, India",
      graduation: "2020"
    )
  ],

  experience: [
    (
      title: "Intern",
      company: "Aimer Society",
      location: "Remote",
      start: "June 2024",
      end: "August 2024"
    ),
    (
      title: "Training & Placement Volunteer",
      company: "Sagi Rama Krishnam Raju Engineering College",
      location: "Bhimavaram, India",
      start: "2024",
      end: "Present"
    )
  ],

  certifications: [
    "Introduction to Artificial Intelligence – Great Learning – 2024",
    "Certificate of Appreciation – NxtWave AI Workshop",
    "Certificate of Appreciation – Sankalp2k24 Arena Winner"
  ],

  soft_skills: [
    "Effective Communication Skills",
    "Decision Making",
    "Time Management",
    "Leadership Qualities"
  ],

  projects: [
    (
      title: "Visual Question & Answering",
      year: "2024",
      description: "Developed an AI model capable of answering questions based on an image input. The system integrates computer vision to interpret visual content and natural language processing to understand and respond to text-based questions, demonstrating the intersection of AI’s perception and language understanding capabilities."
    )
  ]
)

((* set page_numbering_template_placeholders = {
    "NAME": cv.name,
    "PAGE_NUMBER": "\" + str(here().page()) + \"",
    "TOTAL_PAGES": "\" + str(counter(page).final().first()) + \"",
    "TODAY": today
} *))
((* set last_updated_date_template_placeholders = {
    "TODAY": today,
} *))
#import "@preview/fontawesome:0.5.0": fa-icon

#let name = "<<cv.name|remove_typst_commands>>"
#let locale-catalog-page-numbering-style = context { "<<locale.page_numbering_template|replace_placeholders_with_actual_values(page_numbering_template_placeholders)>>" }
#let locale-catalog-last-updated-date-style = "<<locale.last_updated_date_template|replace_placeholders_with_actual_values(last_updated_date_template_placeholders)>>"
#let locale-catalog-language = "<<locale.language>>"
#let design-page-size = "<<design.page.size>>"
#let design-colors-text = <<design.colors.text.as_rgb()>>
#let design-colors-section-titles = <<design.colors.section_titles.as_rgb()>>
#let design-colors-last-updated-date-and-page-numbering = <<design.colors.last_updated_date_and_page_numbering.as_rgb()>>
#let design-colors-name = <<design.colors.name.as_rgb()>>
#let design-colors-connections = <<design.colors.connections.as_rgb()>>
#let design-colors-links = <<design.colors.links.as_rgb()>>
#let design-section-titles-font-family = "<<design.section_titles.font_family>>"
#let design-section-titles-bold = <<design.section_titles.bold|lower>>
#let design-section-titles-line-thickness = <<design.section_titles.line_thickness>>
#let design-section-titles-font-size = <<design.section_titles.font_size>>
#let design-section-titles-type = "<<design.section_titles.type>>"
#let design-section-titles-vertical-space-above = <<design.section_titles.vertical_space_above>>
#let design-section-titles-vertical-space-below = <<design.section_titles.vertical_space_below>>
#let design-section-titles-small-caps = <<design.section_titles.small_caps|lower>>
#let design-links-use-external-link-icon = <<design.links.use_external_link_icon|lower>>
#let design-text-font-size = <<design.text.font_size>>
#let design-text-leading = <<design.text.leading>>
#let design-text-font-family = "<<design.text.font_family>>"
#let design-text-alignment = "<<design.text.alignment>>"
#let design-text-date-and-location-column-alignment = <<design.text.date_and_location_column_alignment>>
#let design-header-photo-width = <<design.header.photo_width>>
#let design-header-use-icons-for-connections = <<design.header.use_icons_for_connections|lower>>
#let design-header-name-font-family = "<<design.header.name_font_family>>"
#let design-header-name-font-size = <<design.header.name_font_size>>
#let design-header-name-bold = <<design.header.name_bold|lower>>
#let design-header-small-caps-for-name = <<design.header.small_caps_for_name|lower>>
#let design-header-connections-font-family = "<<design.header.connections_font_family>>"
#let design-header-vertical-space-between-name-and-connections = <<design.header.vertical_space_between_name_and_connections>>
#let design-header-vertical-space-between-connections-and-first-section = <<design.header.vertical_space_between_connections_and_first_section>>
#let design-header-use-icons-for-connections = <<design.header.use_icons_for_connections|lower>>
#let design-header-horizontal-space-between-connections = <<design.header.horizontal_space_between_connections>>
#let design-header-separator-between-connections = "<<design.header.separator_between_connections>>"
#let design-header-alignment = <<design.header.alignment>>
#let design-highlights-summary-left-margin = <<design.highlights.summary_left_margin>>
#let design-highlights-bullet = "<<design.highlights.bullet>>"
#let design-highlights-nested-bullet = "<<design.highlights.nested_bullet>>"
#let design-highlights-top-margin = <<design.highlights.top_margin>>
#let design-highlights-left-margin = <<design.highlights.left_margin>>
#let design-highlights-vertical-space-between-highlights = <<design.highlights.vertical_space_between_highlights>>
#let design-highlights-horizontal-space-between-bullet-and-highlights = <<design.highlights.horizontal_space_between_bullet_and_highlight>>
#let design-entries-vertical-space-between-entries = <<design.entries.vertical_space_between_entries>>
#let design-entries-date-and-location-width = <<design.entries.date_and_location_width>>
#let design-entries-allow-page-break-in-entries = <<design.entries.allow_page_break_in_entries|lower>>
#let design-entries-horizontal-space-between-columns = <<design.entries.horizontal_space_between_columns>>
#let design-entries-left-and-right-margin = <<design.entries.left_and_right_margin>>
#let design-page-top-margin = <<design.page.top_margin>>
#let design-page-bottom-margin = <<design.page.bottom_margin>>
#let design-page-left-margin = <<design.page.left_margin>>
#let design-page-right-margin = <<design.page.right_margin>>
#let design-page-show-last-updated-date = <<design.page.show_last_updated_date|lower>>
#let design-page-show-page-numbering = <<design.page.show_page_numbering|lower>>
#let design-links-underline = <<design.links.underline|lower>>
#let design-entry-types-education-entry-degree-column-width = <<design.entry_types.education_entry.degree_column_width>>
#let date = datetime.today()
