LAW STUFFThis is the CivicLaw Guru project, a citizen-focused legal-education website and AI-driven scenario analyzer. It uses a retrieval-augmented generation (RAG) system with legal explainers and case law to produce structured, educational outputs for users.Project Structurefrontend/: A Next.js application using React and Tailwind CSS.backend/: An Express.js application handling API calls, LLM integration, and database retrieval.docker-compose.yml: An optional file to set up the database and applications with Docker.Getting StartedClone the repository:git clone [your-repo-url]
cd civiclaw-guru

Install dependencies:cd backend && npm install
cd ../frontend && npm install

Set up the database:The backend requires a Postgres database with the pgvector extension. You can use the provided docker-compose.yml file to get a local instance running.Run the SQL queries from backend/migrations.sql to create the necessary tables.Configure environment variables:Create a .env file in the backend/ directory based on backend/.env.example.Set your OPENAI_API_KEY and DATABASE_URL.Start the applications:# In the backend directory
npm run dev

# In the frontend directory
npm run dev

Usage:The frontend will be available at http://localhost:3001.Enter a scenario in the provided form and click "Analyze" to see the AI-generated legal insights.Legal and Ethical DisclaimerEducational Content Only: This application provides educational content and is not a substitute for legal advice.Privacy: User-provided facts are redacted of Personally Identifiable Information (PII) before being sent to the AI model.Content Sourcing: Content is sourced from public legal resources like LawForIndians and IndianKanoon. The application paraphrases and links to original sources, respecting their terms of use.
