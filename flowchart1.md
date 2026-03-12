```mermaid
flowchart TD
    A([Start]) --> B[Input jumlah data n]
    B --> C[Input semua nilai ke array]
    C --> D[Set max = data[0]]
    D --> E[Set min = data[0]]
    E --> F[i = 1]

    F --> G{i < n ?}

    G -->|Yes| H{data[i] > max?}
    H -->|Yes| I[max = data[i]]
    H -->|No| J{data[i] < min?}

    I --> J
    J -->|Yes| K[min = data[i]]
    J -->|No| L[i = i + 1]

    K --> L
    L --> G

    G -->|No| M[Output max dan min]
    M --> N([End])