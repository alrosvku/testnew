Creating a diagram that uses all of the available formatting and display options in Mermaid might not be feasible, as it would be too complex and difficult to understand. However, I can provide you with a comprehensive example that demonstrates various formatting and display options in Mermaid, such as nodes, relationships, different shapes, and styles.

Here's a sample Mermaid diagram that incorporates various options:
```
mermaid
graph TB
    subgraph Cluster A
        style Cluster A fill:#f9f9f9,stroke:#333,stroke-width:1px
        A[<b>Node A</b><br><i>with italic</i><br><font color="red">red text</font>] -->|Edge Label| B(Flowchart shape)
        A -.Dashed Line.-> C(Rounded<br>Rectangle)
    end

    subgraph Cluster B
        style Cluster B fill:#f0f0f0,stroke:#333,stroke-width:1px
        D{Decision Node} -->|Yes| E["Text Node<br>with <code>code</code>"]
        D -->|No| F>Asymmetrical<br>Shape]
        E --> F
    end

    class A,B,C,D,E,F node-class
    classDef node-class fill:#eef,stroke:#333,stroke-width:2px,font-family:Arial
    class ClusterA,ClusterB cluster-class
    classDef cluster-class font-size:16px,font-weight:bold,font-family:Arial
    click A "https://example.com" "Node A Tooltip"

    linkStyle 0 stroke:#ff3e6c,stroke-width:2px
    linkStyle 1 stroke:#42b983,stroke-width:2px,stroke-dasharray: 5, 5
    linkStyle 2 stroke:#f4a261,stroke-width:2px
    linkStyle 3 stroke:#6c757d,stroke-width:2px
    linkStyle 4 stroke:#ff9e80,stroke-width:2px
```

This example demonstrates the following options:

- Creating subgraphs (clusters) with custom styles.
- Formatting node text with HTML tags.
- Different node shapes (rectangle, rounded rectangle, flowchart shape, etc.).
- Directed and dashed edges with labels.
- Decision nodes (diamond shape).
- Styling nodes and clusters using class definitions.
- Adding click events and tooltips to nodes.
- Customizing edge styles (color, stroke width, dash pattern).

Remember, Mermaid provides many more features and options, so feel free to explore the documentation for more advanced usage: https://mermaid-js.github.io/mermaid/#/
