# NeoGraph Insight

A graph-powered web app that visualizes student collaboration patterns using Neo4j. Built during a campus hackathon to explore how graph databases can uncover hidden relationships and improve team dynamics.

## 🔍 Real-World Problem

During student hackathons, team formation often lacks visibility. Some students collaborate repeatedly, while others remain isolated. I wanted to solve this by:
- Mapping who worked with whom
- Identifying frequent collaborators
- Highlighting students who could benefit from mentorship

## 🛠️ Tech Stack

- **Neo4j AuraDB** – Cloud-hosted graph database
- **Cypher Query Language** – For querying relationships
- **Tailwind CSS + CKEditor** – For clean UI and editable documentation
- **Express.js + Node.js** – Backend API integration

## 📊 Features

- Add nodes and relationships dynamically
- Run Cypher queries to explore graph patterns
- Visualize relationship depth and direction
- Export query results for documentation

## 🧪 Sample Cypher Queries

```cypher
MATCH (a:Student)-[:COLLABORATED_WITH]->(b:Student) RETURN a.name, b.name;
MATCH (s:Student)-[:PART_OF]->(t:Team) RETURN s.name, t.name;

📁 Use Case
I used Neo4j to model student collaboration networks during a hackathon at SDIET. The graph revealed clusters of frequent collaborators and helped organizers identify isolated students to pair with mentors.

📝 Learnings
Graph modeling is more intuitive than table joins for relationship-heavy data.

AuraDB’s cloud interface made setup and scaling effortless.

Cypher’s pattern-matching syntax is a game-changer for querying.

🏆 Certification
I earned the Neo4j Certified Professional credential through GraphAcademy. You can view my progress on my public profile.

🔗 Live Demo & Docs
Coming soon. Meanwhile, feel free to explore the code and contribute.
