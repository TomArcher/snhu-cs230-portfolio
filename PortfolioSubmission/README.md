# Portfolio Submission

This project includes the completed [software design document](./CS230-Project-Software-Design.docx) that I created for my client, The Gaming Room.

**Briefly summarize The Gaming Room client and their software requirements. Who was the client? What type of software did they want me to design?**

The Gaming Room was our client, a company that had already developed *Draw It or Lose It*, an Android-based game similar to the 1980s television show *Win, Lose or Draw*. They wanted us to design a web-based, multi-platform expansion of their existing game that would support Windows, Mac, Linux, and mobile devices while maintaining cross-platform compatibility. The software needed to support multiple concurrent games with teams and players, render stock images progressively over 30-second intervals, enforce unique naming for games and teams, and ensure only single game instances existed in memory at any time.

**What did I do particularly well in developing this documentation?**

I excelled at creating comprehensive platform evaluations that considered multiple perspectives including cost, scalability, and technical requirements for each operating environment. My analysis of memory management strategies, particularly the progressive loading approach with dual-resolution images, demonstrated my technical understanding while keeping the system practical and implementable. The documentation maintained consistency across all three project phases while building systematically from requirements through design constraints to final recommendations, creating a cohesive narrative where I justified each architectural decision.

**What about the process of working through a design document did I find helpful when developing the code?**

Working through the design document forced me to think systematically about the architecture before writing any code, which prevented costly refactoring later. Earlier in my career, I had the tendency to jump into the editor and start coding without a firm understanding of the requirements. Creating the UML diagrams and domain model clarified the relationships between Game, Team, and Player entities, making the implementation of inheritance and composition patterns straightforward. Having documented design patterns like Singleton and Iterator upfront meant I understood exactly why each pattern was necessary and how it solved specific requirements, leading to cleaner, faster, and more purposeful code implementation.

**If I could choose one part of my work on these documents to revise, what would I pick? How would I improve it?**

I would revise the Security section in the Recommendations to be more specific about implementation details rather than listing general security measures. For example, instead of broadly mentioning OAuth 2.0 and encryption, I would provide concrete examples of how player authentication would work, detail the specific data that needs encryption, and create a clear security architecture diagram showing how different platforms would authenticate with the central game server. This would make the security recommendations more actionable for the development team.

**How did I interpret the user's needs and implement them into my software design? Why is it so important to consider the user's needs when designing?**

I interpreted The Gaming Room's needs by focusing on their core challenge: expanding from a single platform to multiple platforms while maintaining game consistency and supporting potentially viral growth. This led to recommending a cloud-based architecture that could scale automatically and the progressive image loading strategy that would work across devices with varying capabilities. Considering user needs is crucial because software that doesn't solve actual user problems, regardless of technical elegance, ultimately doesn't sell. By prioritizing the client's need for cross-platform play and scalability, every design decision aligned with their business goals rather than just technical preferences.

**How did I approach designing software? What techniques or strategies would I use in the future to analyze and design a similar software application?**

I approached the design by first thoroughly understanding the requirements, then evaluating multiple platform options through systematic comparison matrices, and finally synthesizing findings into actionable recommendations. I used established design patterns to solve common problems and created visual models (UML diagrams) to clarify system structure before implementation. In future similar projects, I would continue using evaluation matrices for platform comparison, implement proof-of-concept prototypes earlier to validate architectural decisions, and engage in more iterative design reviews with stakeholders. I would also incorporate cloud-native design principles from the start, considering serverless architectures and microservices as primary options rather than traditional monolithic approaches.