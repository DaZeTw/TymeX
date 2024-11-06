# Meeting Scheduler System

This Meeting Scheduler System is designed to help multiple users schedule meetings based on their availability, preferences, and constraints provided through natural language. It interprets the input, finds overlapping time slots, and suggests the best available times. This system is suitable for use via a Web Portal, Mobile App, or Chat Interface and integrates optional calendar synchronization features.

## System Components

### Answer to Question 2: Functions and Descriptions of Each Component

1. **Users**
   - **Function**: Users provide their availability and constraints through messages.
   - **Description**: Represents individuals inputting their schedule preferences and constraints.

2. **User Interface**
   - **Function**: Captures messages from users and routes them to the NLP Module.
   - **Description**: Acts as a bridge between users and the backend, allowing users to enter their availability in natural language.

3. **NLP Module**
   - **Function**: Extracts relevant availability information from user messages using natural language processing.
   - **Description**: Parses user input to interpret dates, times, preferences, and constraints, then converts them into a structured format.

4. **JSON Files**
   - **Function**: Stores structured availability and constraint data in a readable format for easy access and processing.
   - **Description**: Acts as the primary storage system for user availability and constraints, saved in JSON format for easy integration with other components.

5. **Management System**
   - **Function**: Analyzes the data in JSON files, identifies overlapping time slots, and generates scheduling suggestions.
   - **Description**: Responsible for processing user availability and constraints, finding suitable meeting times, and sending responses back through the User Interface.

## System Workflow

1. **User Input**: Users enter availability and preferences through the User Interface (web, mobile, or chat).
2. **NLP Parsing**: The NLP Parsing Module interprets the natural language input and converts it into structured JSON data.
3. **Availability Management**: Parsed data is stored and managed in JSON format.
4. **Scheduling**: The Management System finds overlapping availability, prioritizes according to preferences, and suggests the best meeting time.
5. **User Confirmation**: Suggested times are displayed through the User Interface for user review.
6. **Finalization**: Once a time slot is confirmed, notifications are sent to all participants.
7. **Calendar Integration (Optional)**: If enabled, the system adds the meeting to users’ Google or Outlook calendars.
