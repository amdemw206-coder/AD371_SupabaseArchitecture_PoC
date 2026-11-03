# AD371_SupabaseArchitecture_PoC 

### Project Description: 
- Application Analysed: Supabase
- Prototype built: PoC lightweight HTML application that details on the architectural components of Supabase that allows it to operate as a Backend-as-a-Service (BaaS).

### Setup & Run Instructions: 
- (i) Navigate to "PoC files"
- (ii) Right-click on "supabase_architectural_dashboard_poc.html" hover on "Open With" and select your preferred browser
    - *Something to note*: the file "supabase_architectural_dashboard_poc_with_original_flaws.html" is the original AI assisted file that was scaffolded to create the html file from step 2.  

### AI Disclosure and Prompt Appendix: 
- AI Tool Used: Gemini   
- Sample Prompt Used: 
    - Use an LLM to generate an initial breakdown of the system and scaffold a lightweight companion application (e.g., an architectural dashboard, an API client interfacing with the open-source tool, or a functional PoC recreating one subsystem like authentication or queue processing)
- Initial Prompt Generated: supabase_architectural_dashboard_poc_with_original_flaws.html (./PoCfiles)
- Summary of Corrections: 
    - AI Fact-Check: 
        - (i) In the Request Flow Visualizer page, it incorrectly identifies the API gateway as “Kong,” which was recently replaced by Envoy in August 2026. 
        - (ii) Core Component Matrix page is missing a few architecture components:  Studio dashboard, postgres-meta API, Supervisor as connection pooler (which does appear in Request Flow Visualizer page),and Envoy API Gateway (which if it did appear in the matrix I would assume it would be Kong) 
    - Customizing: 
        - (i) Tailwind CSS color edits to match the look of Supabase.
        - (ii) Getting rid of elements that bloat the Proof of Concept page (mainly from the header).
        - (iii) Updating core component matrix page to add all architecture components.
 
