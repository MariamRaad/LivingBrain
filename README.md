# Living Brain - Software Engineering Portfolio

> ⚠️ **Disclaimer**
>
> This repository is a personal portfolio showcasing selected work and contributions from my time at **living brain GmbH**.
>
> Due to confidentiality, intellectual property, and data protection requirements, this repository does **not** contain proprietary source code, internal documentation, patient data, customer data, or other confidential company information.
>
> The examples, screenshots, videos, and descriptions shown here have been carefully selected and anonymized where necessary. They are intended to demonstrate my technical experience, responsibilities, and contributions without exposing confidential company information.
>
> All rights to the original products, software, assets, trademarks, and other intellectual property remain with their respective owners.

---

## My Role

I joined living brain in 2020 and progressed from an internship to a Senior Software Engineer role.

| Period | Role |
|---|---|
| Sep 2020 – Aug 2021 | **Unity 3D Developer (Internship)** |
| Sep 2021 – Aug 2023 | **Junior Unity Developer** |
| Sep 2023 – Sep 2024 | **Unity Developer** |
| Oct 2024 – Sep 2026 | **Senior Software Engineer** |

During my time at living brain, I worked across software development, product development as well as selected quality and regulatory activities.

I mainly worked with:

C# · Unity 3D · Visual Studio · .NET / WPF · Meta Quest · Pico · Git / GitHub / Plastic SCM · Audacity · Confluence · Jira · Scrum

My work covered:

- Unity 3D software development
- Feature planning, design and implementation
- VR training environments and interactive scenarios
- Audio and sound design, integration and implementation
- Localization and multilingual application support
- Software maintenance and further development
- Internal tools and software libraries
- Debugging and problem solving
- Software documentation
- Technical customer support via email, phone and on-site
- Quality Management, validation and product testing
- Regulatory and medical-device-related activities
- Product testing and audit support
- Organizational and administrative support

---

# Projects

## 1. teora® mind

### Overview

teora® mind is a VR therapy software for cognitive training in clinical rehabilitation and at-home aftercare. It is designed to help people with neurological conditions train cognitive abilities such as memory, attention and concentration through realistic and everyday activities.

Instead of relying primarily on abstract cognitive exercises, teora® mind uses immersive virtual environments to recreate familiar real-world situations. Users can practice activities based on **Activities of Daily Living (ADLs)**, such as preparing coffee, handling groceries or preparing food, in a safe and repeatable environment. The application can be used in conjunction with **teora® platform**, a web-based patient management and therapy management solution that allows therapists to create individual training plans and exchange relevant training data with teora® mind.

The application consists of multiple interactive environments and exercises, including a kitchen, beach and garden, as well as dedicated mini-games. In total, the product includes **17 exercises and 3 mini-games**.

I worked on teora® mind throughout my entire time at living brain, contributing to the development and continuous evolution of the application as a Unity Developer / Software Engineer.

As a medical device, teora® mind was developed within a regulated environment and is a **Class IIa medical device under the European Medical Device Regulation (MDR)**. In addition to software development, I was involved in quality management and regulatory activities, including software validation, product testing, documentation, QMS changes, and the planning, preparation and support of internal and external audits.

### General Work

Across the different environments and exercises of teora® mind, I was regularly involved in the implementation and setup of new and existing scenes.

This included:  
- Implementing and maintaining **level and scene structures**, including colliders, respawn areas and scene-specific setup
- Developing and maintaining the **in-game tablet UI** and its application-wide features
- Editing, integrating and configuring **audio and sound systems** across scenes and interactive objects
- Implementing and maintaining **localization** with multilanguage content, including texts, assets, a language selection and RTL support
- Supporting **multiple VR headsets**, including Meta Quest 2, Quest 3S and Pico 4
- Implementing and adapting **VR interaction and UI systems**, including pointers, raycasts and controller-specific UI hints
- Developing reusable and configurable systems and components using **ScriptableObjects** and **Prefabs**
- Implementing application-wide features such as **pause tracking, scene transitions and device status information**
- Integrating features for communication with **teora® platform** and other parts of the teora® ecosystem
- Adapting and reworking existing gameplay and interaction systems to new environments
- Managing and integrating Unity and SDK / plugin updates
- Troubleshooting and maintaining existing scenes and features
- Collaborating with artists to integrate and iterate on visual effects and gameplay feedback

### Selected Work

#### 1. Minigame Shooting (Prototype)

I developed gameplay features and interactive systems for a shooting-based VR minigame. This level was still under development and was not completed as a finished product.

The prototype combines shooting mechanics, interactive objects, physics-based interactions and timed gameplay events into a playable VR experience. In each playthrough the targets spawn at random locations which makes every playthrough unique.

**My contribution included:**
- Developing the **scoring and timer systems**, including difficulty-dependent timing and a wave-based level completion condition
- Implementing the **nailgun interaction and shooting feedback**, including projectile particle trails
- Developing interactive shootables and their individual behaviors, including:
  - **Moving robot** following a defined path
  - **Jack-in-the-box** with opening/closing lid, physics-based jumping behavior as well as reactions when hit
  - **Ice block** with hit feedback and progressive crack decals
  - **Balloons** with spawning, movement, scaling and hit effects
  - **UFO shield** with projectile interaction and visual hit feedback
- Implementing the **Freeze Event**, temporarily pausing affected gameplay objects through their physics state

https://github.com/user-attachments/assets/ae4ec8d4-c3bb-41bc-b841-8bbba5957583

#### 2. Custom Cable System

For the kitchen environment, I developed a custom physics-based cable system to replace the previously used third-party solution.

The goal was to reduce external dependencies while having more control over the system and its behavior.

**My contribution:**
- Designed and implemented the cable system using Unity physics, rigidbodies and joints
- Created the cable mesh procedurally based on the physical cable structure
- Integrated the system with existing VR interactions
- Designed the cable behavior with **user experience in mind**, including automatic retraction when the cable is stretched too far
- Tested and evaluated the performance using Meta's OVR Metrics Tool in comparison to the previously used third-party plugin

The result was a reusable cable solution that could be integrated into the existing kitchen interactions without relying on the previous third-party plugin.

[Video / GIF]

#### 3. Tutorial Rework

The existing tutorial flow was completely replaced with a new concept consisting of a guided tutorial and a separate recycling section. We wanted to provide a clearer and more accessible introduction to the VR application.

The result was a more structured onboarding experience that gradually introduced users to the application's interactions and mechanics.

**My contribution:**
- Reworked the existing gameplay and scene structure
- Extended and adapted the existing quest system
- Implemented new UI panels and visual guidance
- Integrated and controlled animations programmatically
- Adapted existing interaction logic to the new gameplay flow

[Video / GIF]

#### 4. Audio & Sound Integration

I worked closely with another developer on the audio system used throughout teora® mind. While the underlying sound system was developed by my colleague, we collaborated on its design and integration into the application. The system used a material-based sound matrix with **50+ sound combinations**, covering different material interactions for collision sounds as well as grab and snap sounds for interactable objects.

Particular attention was given to creating believable audio feedback for different materials and interactions, helping to make physical interactions in VR feel more natural and immersive.

**My contribution:**
- Researched and selected suitable sound effects, including a large library of material-specific sounds
- Edited and prepared audio assets using Audacity
- Established workflows and naming conventions for organizing and integrating audio assets
- Organized sounds based on material and interaction type
- Integrated and configured sound components across scenes and reusable prefabs
- Continuously maintained and extended the audio setup as new content was added

[Video / GIF]

#### 5. Localization

TODO

---

## 2. teora® body

### Overview

Brief description of the product and its purpose.

TODO it has Hand Tracking, in comparison to teora mind

- VR interactions
- Gameplay mechanics
- Physics-based interactions
- Hand tracking
- Haptics
- Modular prefabs
- UI / UX
- Localization
- Audio integration

### General Work

TODO write that down differently than in teora mind text above
Across the different environments and exercises of teora® body, I was regularly involved in the implementation and setup of new and existing scenes.  
This included:  
- TODO

### Selected Work

#### 1. [Most impressive work result]

Short description.

[Video / GIF]

#### 2. [Second work result]

Short description.

[Video / GIF]

#### 3. [Third work result]

Short description.

[Video / GIF]

---

## 3. Device Setup Tool

### Overview

Brief description of the internal tool and its purpose.
TODO WPF project

### Selected Work

#### 1. [Most impressive work result]

Short description.

[Video / GIF]

---
