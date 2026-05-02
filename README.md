# Riverside

Riverside is a professional podcast and video recording platform that enables remote studio-quality recording, AI-powered editing, and publishing. The Riverside Business API provides programmatic access to recordings, productions, studios, projects, exports, transcriptions, and webinar management for enterprise podcast production workflows. API access is available on the Business plan only.

**Website:** [https://riverside.fm](https://riverside.fm)

**Documentation:** [https://docs.riverside.fm/](https://docs.riverside.fm/)

## APIs

### Riverside Business API

The Riverside Business API provides programmatic access to recording management, production workflows, studio and project organization, file downloads, transcription retrieval, export management, and webinar registration. Authentication uses API key bearer tokens.

- **Base URL:** `https://platform.riverside.fm`
- **Authentication:** API Key (Bearer Token)
- **Documentation:** [https://docs.riverside.fm/endpoints-reference/v3/](https://docs.riverside.fm/endpoints-reference/v3/)
- **Getting Started:** [https://support.riverside.fm/hc/en-us/articles/9068592900381-Riverside-Business-API](https://support.riverside.fm/hc/en-us/articles/9068592900381-Riverside-Business-API)

#### Endpoints

| Method | Path | Description |
|--------|------|-------------|
| GET | `/api/v3/productions` | List workspace productions with studios and projects |
| GET | `/api/v2/recordings` | List all recordings with filters |
| GET | `/api/v1/recordings/{recording_id}` | Get a specific recording with tracks |
| DELETE | `/api/v1/recordings/{recording_id}` | Delete a recording |
| GET | `/api/v1/recordings/{recording_id}/transcription/download` | Download transcription (SRT/TXT) |
| GET | `/api/v1/exports` | List all exports |
| GET | `/api/v1/exports/{export_id}` | Get a specific export |
| DELETE | `/api/v1/exports/{export_id}` | Delete an export |
| GET | `/api/v1/exports/{export_id}/download` | Download export file |
| POST | `/api/v1/webinars/{webinar_id}/registrants` | Register a webinar participant |
| GET | `/api/v1/webinars/{webinar_id}/registrants` | List webinar registrants |

## Artifacts

### OpenAPI Specifications

| Spec | Description |
|------|-------------|
| [openapi/riverside-business-openapi.yml](openapi/riverside-business-openapi.yml) | Riverside Business API — recordings, productions, exports, transcriptions, webinars |

### Spectral Rules

| Ruleset | Description |
|---------|-------------|
| [rules/riverside-business-rules.yml](rules/riverside-business-rules.yml) | Riverside API linting rules enforcing versioned paths, rate limit documentation |

### Capabilities

| Capability | Description |
|------------|-------------|
| [capabilities/podcast-production.yaml](capabilities/podcast-production.yaml) | Unified workflow for enterprise podcast and video production |
| [capabilities/shared/riverside-business.yaml](capabilities/shared/riverside-business.yaml) | Shared Riverside Business API consumed definition |

### JSON Schemas

| Schema | Description |
|--------|-------------|
| [json-schema/riverside-recording-schema.json](json-schema/riverside-recording-schema.json) | Recording object with tracks, transcription, and metadata |

### JSON Structure

| Structure | Description |
|-----------|-------------|
| [json-structure/riverside-recording-structure.json](json-structure/riverside-recording-structure.json) | Field-by-field documentation of the recording object |

### JSON-LD Context

| Context | Description |
|---------|-------------|
| [json-ld/riverside-context.jsonld](json-ld/riverside-context.jsonld) | Linked data context mapping Riverside terms to schema.org |

### Examples

| Example | Description |
|---------|-------------|
| [examples/riverside-list-recordings-example.json](examples/riverside-list-recordings-example.json) | List workspace recordings with paginated response |

### Vocabulary

| Vocabulary | Description |
|------------|-------------|
| [vocabulary/riverside-vocabulary.yml](vocabulary/riverside-vocabulary.yml) | Podcast production terms including Recording, Studio, Production, Transcription |

## Tags

Podcast, Video Recording, Media, Content Creation, Audio

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
