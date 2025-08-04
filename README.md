Travel Planner AI Agent
An intelligent assistant built using IBM Watsonx + Granite LLM + RAG
IBM Hackathon Submission – Agentic AI Challenge 2025
By Soham Gore | K. J. Somaiya School of Engineering, Computer Engineering

Project Overview
The Travel Planner AI Agent helps users plan their trips smartly using an AI assistant that can answer natural language questions like:

“Where can I travel in December under ₹10,000?”
“What are must-visit places in Goa?”
“Suggest a 3-day itinerary for Manali.”

This agent uses a Retrieval-Augmented Generation (RAG) approach powered by IBM Watsonx and Granite Foundation Models. It retrieves grounded travel knowledge from a custom dataset and generates accurate, contextual responses.

Problem Statement (No. 5 – Travel Planner Agent)
A Travel Planner Agent is an AI-powered assistant that helps users plan trips efficiently and intelligently.
It uses real-time data to suggest destinations, build itineraries, and recommend transport and accommodation options.
By understanding user preferences and constraints, it tailors personalized travel plans.

Tech Stack
Component	Details
AI Model	IBM Granite 13B-Instruct (via Watsonx Studio)
Retrieval	Watsonx Vector Index with custom .txt dataset
Platform	IBM Cloud Lite
Search Strategy	Semantic Search using RAG
Dataset	travel_knowledge.txt (23+ Indian destinations)
Tools	Watsonx AI Studio, IBM Object Storage

Dataset: travel_knowledge.txt
The knowledge base includes travel tips for 20+ Indian destinations:

Best time to visit

Budget range

Top attractions

Planning tips

This file is uploaded into Watsonx Studio as a vector index for grounding LLM responses.

How It Works
Upload travel_knowledge.txt to Watsonx Vector Index
Create agent using Watsonx Studio (Granite-13B-Instruct)
User types a travel query in plain English
Agent retrieves relevant data and generates a custom response
Agent can be deployed and integrated via Watsonx APIs



Deployment status (Watsonx Studio)

Sample Queries
User Query	Example Answer
"What’s the best time to visit Jaipur?"	October to March
"Cheap places to visit in November?"	Rishikesh, Mysore, Pondicherry
"What to do in Manali?"	Rohtang Pass, Solang Valley, Hidimba Temple


Future Scope
Add real-time APIs for weather and hotel bookings

Voice-based assistant with IBM Speech-to-Text

Integration with WhatsApp or web UI

Multilingual support using IBM Language Translator

User preference profiling and session memory

