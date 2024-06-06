---
order: 88
icon: list-ordered
label: Static Data
---

# Static Data

## Language Codes & Localization

| Language | Description                |
|----------|----------------------------|
| zh       | Simplified Chinese         |
| zh-hk    | Traditional Chinese        |
| pt-br    | Brazilian Portuguese       |
| es       | Castilian Spanish          |
| es-la    | Latin American Spanish     |
| ja-ro    | Romanized Japanese         |
| ko-ro    | Romanized Korean           |
| zh-ro    | Romanized Chinese          |
| en       | English                    |
| ja       | Japanese                   |
| ko       | Korean                     |
| fr       | French                     |
| de       | German                     |
| ru       | Russian                    |
| it       | Italian                    |
| es       | Spanish                    |
| pt       | Portuguese                 |
| nl       | Dutch                      |
| pl       | Polish                     |
| tr       | Turkish                    |
| ar       | Arabic                     |
| th       | Thai                       |
| vi       | Vietnamese                 |

## Manga publication demographic

| Value   | Description        |
|---------|--------------------|
| shounen | Manga is a Shounen |
| shoujo  | Manga is a Shoujo  |
| josei   | Manga is a Josei   |
| seinen  | Manga is a Seinen  |

## Manga status

| Value     | Description              |
|-----------|--------------------------|
| ongoing   | Manga is still going on  |
| completed | Manga is completed       |
| hiatus    | Manga is paused          |
| cancelled | Manga has been cancelled |

## Manga content rating

| Value        | Description          |
|--------------|----------------------|
| safe         | Safe content         |
| suggestive   | Suggestive content   |
| erotica      | Erotica content      |
| pornographic | Pornographic content |

## Manga order options

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
| img_cover        | A Image Cover for a manga `*`    |
| author           | Author resource                |
| artist           | Author resource (drawers only) |
| scanlation_group | ScanlationGroup resource       |
| tag              | Tag resource                   |
| user             | User resource                  |
| custom_list      | CustomList resource            |

## Manga links data

In Manga attributes you have the `links` field that is a JSON object with some strange keys, here is how to decode this
object:

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
