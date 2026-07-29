# Plantix-Demo

A simple Android application that demonstrates fetching data from a REST API using Retrofit, handling asynchronous tasks with Coroutines, and displaying a list of items with images.

## 🚀 Features

- **API Integration:** Fetches data (rows with title, description, and image) from a JSON endpoint.
- **Image Loading:** Efficiently loads images from URLs using the Glide library.
- **List Display:** Uses `RecyclerView` to display a scrollable list of items.
- **UI Architecture:** Utilizes `ViewBinding` for safer and easier interaction with UI components.
- **Modern Concurrency:** Uses Kotlin Coroutines for off-loading network calls from the main thread.

## 🛠 Tech Stack

- **Language:** Kotlin
- **Network:** [Retrofit 2](https://square.github.io/retrofit/) & OkHttp
- **JSON Parsing:** Gson
- **Image Loading:** [Glide](https://github.com/bumptech/glide)
- **UI Components:** Material Design, RecyclerView, ConstraintLayout
- **Dependency:** SSP & SDP (for scalable units)
- **Other:** ViewBinding, Coroutines

## 📁 Project Structure

```text
app/src/main/java/com/example/plantixdemo/
├── adapters/          # RecyclerView adapters (PlantixDataAdapter)
├── models/            # Data models for API responses (PlantixResponseModel)
├── network/           # Retrofit service interface and API client configuration
├── ui/
│   └── activities/    # Activity classes (MainActivity)
└── utils/             # Helper classes (ProgressDialog)

app/src/main/res/
├── layout/            # XML layout files
└── values/            # String, color, and style definitions
```
### API Endpoint
The app currently fetches data from:
`https://dl.dropboxusercontent.com/s/2iodh4vg0eortkl/facts.json`
