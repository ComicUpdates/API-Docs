---
order: 88
icon: list-ordered
label: Static Data
---

# Static Data

## Language Codes & Localization

| Language | Description                |
|----------|----------------------------|
| en       | English                    |
| zh       | Simplified Chinese         |
| es       | Castilian Spanish          |
| ar       | Arabic                     |
| hi       | Hindi                      |
| bn       | Bengali                    |
| ru       | Russian                    |
| pt       | Portuguese                 |
| id       | Indonesian                 |
| fr       | French                     |
| de       | German                     |
| ja       | Japanese                   |
| ko       | Korean                     |
| it       | Italian                    |
| tr       | Turkish                    |
| pl       | Polish                     |
| ms       | Malay                      |
| pt-br    | Brazilian Portuguese       |
| vi       | Vietnamese                 |
| th       | Thai                       |
| fa       | Persian                    |
| es-la    | Latin American Spanish     |
| nl       | Dutch                      |
| ro       | Romanian                   |
| el       | Greek                      |
| hu       | Hungarian                  |
| no       | Norwegian                  |
| sv       | Swedish                    |
| cs       | Czech                      |
| uz       | Uzbek                      |
| bg       | Bulgarian                  |
| hr       | Croatian                   |
| sk       | Slovak                     |
| da       | Danish                     |
| fi       | Finnish                    |
| he       | Hebrew                     |
| ca       | Catalan                    |
| et       | Estonian                   |
| lt       | Lithuanian                 |
| sl       | Slovenian                  |
| zh-hk    | Traditional Chinese        |
| fil      | Filipino                   |
| uk       | Ukrainian                  |
| sr       | Serbian                    |
| kk       | Kazakh                     |
| mn       | Mongolian                  |
| ne       | Nepali                     |
| ta       | Tamil                      |
| te       | Telugu                     |
| ka       | Georgian                   |
| eo       | Esperanto                  |
| la       | Latin                      |
| az       | Azerbaijani                |
| my       | Burmese                    |
| ja-ro    | Romanized Japanese         |
| ko-ro    | Romanized Korean           |
| zh-ro    | Romanized Chinese          |

## Publication Demographic

| Value   | Description        |
|---------|--------------------|
| shounen | Is a Shounen       |
| shoujo  | Is a Shoujo        |
| josei   | Is a Josei         |
| seinen  | Is a Seinen        |

## Status

| Value     | Description              |
|-----------|--------------------------|
| ongoing   | Is still going on        |
| completed | Is completed             |
| hiatus    | Is paused                |
| cancelled | Has been cancelled       |

## Content rating

| Value        | Description          |
|--------------|----------------------|
| safe         | Safe content         |
| suggestive   | Suggestive content   |
| erotica      | Erotica content      |
| pornographic | Pornographic content |

## Order options

| Name                  | Value                   | Default  |
|-----------------------|-------------------------|----------|
| title                 | Enum: `"asc"`, `"desc"` |          |
| year                  | Enum: `"asc"`, `"desc"` |          |
| createdAt             | Enum: `"asc"`, `"desc"` |          |
| updatedAt             | Enum: `"asc"`, `"desc"` |          |
| latestUploadedChapter | Enum: `"asc"`, `"desc"` | `"desc"` |
| followedCount         | Enum: `"asc"`, `"desc"` |          |
| relevance             | Enum: `"asc"`, `"desc"` |          |

## Chapter order options

| Name       | Value                   | Default |
|------------|-------------------------|---------|
| createdAt  | Enum: `"asc"`, `"desc"` | `"asc"` |
| updatedAt  | Enum: `"asc"`, `"desc"` | `"asc"` |
| publishAt  | Enum: `"asc"`, `"desc"` | `"asc"` |
| readableAt | Enum: `"asc"`, `"desc"` | `"asc"` |
| volume     | Enum: `"asc"`, `"desc"` | `"asc"` |
| chapter    | Enum: `"asc"`, `"desc"` | `"asc"` |

## Relationship types

| Value            | Description                    |
|------------------|--------------------------------|
| manga            | Manga resource                 |
| chapter          | Chapter resource               |
| img_cover        | A Image Cover for a manga      |
| author           | Author resource                |
| artist           | Author resource (drawers only) |
| scanlation_group | ScanlationGroup resource       |
| tag              | Tag resource                   |
| user             | User resource                  |
| custom_list      | CustomList resource            |

## Links data

The `links` field in Manga attributes contains a JSON object with some strange values. The following describes how to decode this object:

| Key   | Related site  | URL                                                                                           | URL details                                                    |
|-------|---------------|-----------------------------------------------------------------------------------------------|----------------------------------------------------------------|
| ebj   | ebookjapan    | N/A                                                                                           | Stored as full URL                                             |
| cdj   | CDJapan       | N/A                                                                                           | Stored as full URL                                             |
| raw   | N/A           | N/A                                                                                           | Stored as full URL, untranslated stuff URL (original language) |
| engtl | N/A           | N/A                                                                                           | Stored as full URL, official english licenced URL              |

## Manga related enum

This data is used in the "related" field of a Manga relationships

| Value             | Description                                                          |
|-------------------|----------------------------------------------------------------------|
| monochrome        | A monochrome variant of this manga                                   |
| colored           | A colored variant of this manga                                      |
| preserialization  | The original version of this manga before its official serialization |
| serialization     | The official serialization of this manga                             |
| prequel           | The previous entry in the same series                                |
| sequel            | The next entry in the same series                                    |
| main_story        | The original narrative this manga is based on                        |
| side_story        | A side work contemporaneous with the narrative of this manga         |
| adapted_from      | The original work this spin-off manga has been adapted from          |
| spin_off          | An official derivative work based on this manga                      |
| based_on          | The original work this self-published derivative manga is based on   |
| doujinshi         | A self-published derivative work based on this manga                 |
| same_franchise    | A manga based on the same intellectual property as this manga        |
| shared_universe   | A manga taking place in the same fictional world as this manga       |
| alternate_story   | An alternative take of the story in this manga                       |
| alternate_version | A different version of this manga with no other specific distinction |
