# Urban Data Visualization

In recent years, cities have become a huge source of various data. The urban data usually includes building metadata, street layouts, public transport information, layouts of the power network, noise maps, socio-economic maps, etc. The data is usually freely accessible in a format that is obscure for the general public. Naturally, to make the data more accessible, it is necessary to visualize it. Local authorities usually make this effort, with either one of the following goals: to inform the public about the current state or present the effects of a future change in the area. Usually, the visualization is presented in a public space, either in museums or centers specifically equipped for this kind of presentation. While some of these places own the necessary equipment, the production pipeline is often complicated, and an ad-hoc solution is used. In other cases, the visualization is presented using proprietary software, which is not primarily designed for the general public. This thesis presents a novel framework for urban data visualization. This framework aims to give the creators powerful tools and produce simple yet highly customizable outputs comprehensible by the general public. 

Communicating the current state usually requires analysis and simplification of the raw data, and there is a wide range of tools for that. However, these tools are usually proprietary, and the outputs are not that engaging. The visualization is rarely customizable; proprietary formats are used throughout the entire pipeline, and it is impossible to combine various types of data. 

Communicating the future changes is even more difficult since it requires to inform the public about the current state first. In this context, the interactivity of the presentation can be the key to understanding. 

There are several technical challenges. The input data is often in several incompatible formats, and each describes a completely different urban domain. In other words, the datasets are often complementary, and the system has to support their combination. For example, some data use different coordinate systems, or the datasets differ in their dimensionality. 

The aforementioned technical obstacles should remain hidden from both the visualization creator and also the audience. In the ideal case, the visualization creator is given absolute freedom, and the framework does not pose any hard restrictions on what is possible; the creator's imagination is the only limit. This utopistic idea is often contradicted by the requirement of a simple and usable interface. It is appropriate to seek a balance between unlimited possibilities and usability. 

Furthermore, there is an artistic aspect of the visualization. The goal is to make the visualization immersive enough to captivate, educate, and entertain the viewers. The framework's capabilities should not diminish the experience and avoid posing any virtual barriers between the medium and the audience.

The goal is to develop a modular system, which will streamline the urban data visualization process. The design should focus on the following four factors:
* the actual communicated information,
* the nature of the available urban data, 
* the creator's artistic vision, 
* and the equipment used for the presentation. 

The tricky part is that probably only one or two of those factors are known in advance - the urban data and the used equipment can be somewhat standardized. The remaining two factors are usually project-specific; therefore, it is necessary to explore the combination of various data types and somehow (?) enable the freedom of artistic expression. Because of the desired modularity and adjustability, the goal is to build a system for building systems - there is an inherent metaprogramming element. 



