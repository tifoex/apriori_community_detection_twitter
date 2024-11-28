# Community Detection in Social Networks

This project implements a novel approach for detecting communities in social networks by combining user interaction patterns and structural relationships. It aims to provide deeper insights into social network behavior and the roles of users.

## Features
- **Community Detection**: Identifies user groups based on shared interactions and activities.
- **Frequent Pattern Mining**: Extracts recurring user interaction patterns.
- **Hierarchical Clustering**: Forms cohesive sub-communities by merging similar patterns.
- **Network Expansion**: Assigns isolated users to relevant communities using similarity measures.

## Methodology
1. **Data Preprocessing**:
   - Extract user relationships and activities.
   - Generate two main tables:
     - **Relations Table**: Captures directed relationships such as followers.
     - **Activities Table**: Logs actions like mentions, retweets, and replies.

2. **Frequent Pattern Extraction**:
   - Use the Apriori algorithm to discover common interaction patterns.
   - Filter patterns based on a support threshold.

3. **Community Formation**:
   - Evaluate user similarity using multiple metrics (e.g., common followers, mentions).
   - Homogenize patterns and merge similar groups using hierarchical clustering.

4. **Community Expansion**:
   - Assign ungrouped users to communities based on similarity to group leaders or neighbors.

## Dataset
This project utilizes the **Higgs Twitter Dataset**, which includes:
- Data from ~500,000 users.
- Interaction types: followers, retweets, replies, and mentions.

## Results
- Communities were detected with high precision and recall.
- The methodology was compared to the Louvain algorithm and a greedy approach, demonstrating better performance in balancing accuracy and flexibility.

## Project Files
- **Data**: Includes raw data and preprocessing scripts.
- **Code**: Scripts for processing, analysis, and community detection.
- **Results**: Outputs from the community detection process.

## How to Use
1. Preprocess the data to create relations and activities tables.
2. Run the frequent pattern mining to identify recurring user behaviors.
3. Use the detected patterns to form and expand communities.

## Future Improvements
- Handle dynamic networks to detect evolving communities.
- Incorporate additional user attributes and similarity measures.
- Optimize for larger datasets and real-time processing.

## Acknowledgments
This project was conducted in Python using tools like Google Colab for computational efficiency. Special thanks to the creators of the **Higgs Twitter Dataset** for providing the foundation for this research.

## License
This project is released under the MIT License.

## CONTACT US:
alirezaakhavansafaei@gmail.com
studylab.ir
