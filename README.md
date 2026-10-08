# Nutrify — AI-Powered Nutrition Q&A

## Overview

Nutrify is a prototype nutrition question-and-answer application designed to provide users with personalized nutrition guidance. The system combines three knowledge sources: an OpenAI large language model (LLM), a specialized nutrient-analysis model, and a nutrient database.

The project explores how multiple specialized knowledge sources can work together within a modular software architecture to support nutrition-related questions and answers.

## Architecture

Nutrify was designed around the **Blackboard architectural pattern**, which provides a shared workspace for independent knowledge sources to contribute information toward solving a problem.

The proposed architecture includes:

* **Knowledge Sources:** An OpenAI LLM, a specialized nutrient-analysis model, and a nutrient database.
* **Central Forum:** A shared workspace where knowledge sources contribute intermediate responses.
* **Answer Management:** Coordinates expert responses and selects an answer to return to the user.
* **Question Management:** Supports question submission and question-history operations.
* **Account Management:** Handles user accounts, authentication, and account customization.
* **User Success Management:** Collects user ratings to support future improvements.
* **Data Storage:** Separate databases for account information and question-and-answer data.
* **Client Interface:** Provides the user-facing interaction layer.

The team implemented a basic prototype of the application alongside the architectural design.

## Design Rationale

The Blackboard pattern was selected to support modularity and collaboration between specialized knowledge sources. By separating knowledge sources from question handling, answer management, account management, and feedback, the design aimed to make individual components easier to modify and extend.

Alternative architectural styles were evaluated, including Repository, Batch Sequential, Pipe-and-Filter, and Process-Control architectures. The Blackboard approach was selected based on the project's need for coordinated contributions from multiple knowledge sources.

## Key Concepts

* AI and LLM integration
* Multi-source knowledge processing
* Blackboard software architecture
* Subsystem decomposition and separation of concerns
* Architectural trade-off analysis
* User feedback and iterative improvement

## Project Materials

The repository may include the prototype source code, technical report, presentation, and architecture diagrams, depending on the materials available.

## Project Scope

Nutrify was developed as a university software architecture and design project. The implementation was a basic prototype intended to demonstrate the application concept and architectural approach; it was not a production-ready nutrition or medical advice system.

