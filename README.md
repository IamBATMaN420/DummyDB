# DummyDB
**AI-Powered Database Interface That Actually Works**  
*Talk to your database in plain English. No SQL knowledge required. No really, we mean it.*

---

##  What is DummyDB?

DummyDB transforms any database into a conversational partner. Ask questions in natural language, get real data back. Generate dummy datasets with a simple prompt. Query complex relationships without memorizing JOIN syntax.

Built during **Hexafall 2025** after we scrapped our original idea 12 hours in and decided to build something that might actually be useful.

> **"Show me users who haven't logged in for 30 days"**  
> **"Generate 100 fake customers with realistic purchase history"**  
> **"What's our average order value by region?"**

DummyDB understands all of this. Your database finally speaks human.

---

##  Features

 **Natural Language Queries** — Ask questions like you're talking to a data analyst  
 **Smart SQL Generation** — Translates your prompts into optimized database queries  
 **Dummy Data Creation** — Generate realistic test data with custom constraints  
 **Real-time Execution** — See results instantly in a clean, responsive interface  
 **Universal Database Support** — Works with PostgreSQL, MySQL, SQLite, and more  
 **Safe by Design** — Read-only mode and query validation built-in

---

##  Quick Start

### Prerequisites
- Node.js 18+
- A database (we'll use PostgreSQL for this example)
- OpenAI API key

### Installation

```bash
# Clone the repository
git clone https://github.com/ayushbaasak101/dummydb.git
cd dummydb

# Install backend dependencies
npm install

# Install frontend dependencies
cd client && npm install && cd ..
```

### Environment Setup

Create a `.env` file in the root directory:

```env
OPENAI_API_KEY=your_openai_api_key_here
DATABASE_URL=postgresql://username:password@localhost:5432/your_database
NODE_ENV=development
```

### Run the Application

```bash
# Start the backend server
npm run server

# In a new terminal, start the frontend
npm run client

# Or run both simultaneously
npm run dev
```

Visit `http://localhost:3000` and start talking to your database!

---

##  How It Works

1. **You speak human** → *"Find customers who bought more than $500 worth of products last month"*
2. **AI translates** → `SELECT c.name, SUM(o.total) FROM customers c JOIN orders o...`
3. **Database responds** → Clean, formatted results in your browser
4. **You get answers** → No SQL required, no schema memorization needed

---

##  Tech Stack

**Frontend**
- React 18 with Hooks
- TailwindCSS for styling
- Recharts for data visualization

**Backend**
- Node.js + Express
- OpenAI GPT-4 API integration
- Database connection pooling

**Database Support**
- PostgreSQL (primary)
- MySQL, SQLite, SQL Server (tested)
- Easy to extend for other SQL databases

---

##  Example Queries

```
"How many users signed up this week?"
"Show me the top 5 products by revenue"
"Generate 50 fake orders for testing"
"Which customers haven't ordered in 6 months?"
"Create sample data for a blog with posts and comments"
```

---

##  Demo

**[▶ Watch the full demo on YouTube](https://youtu.be/So2pXvAbr40?si=48p0VMBOlP2NoraL)**

See DummyDB in action, from natural language input to real database results.

---

##  Safety Features

- **Read-only mode** available for production databases
- **Query validation** prevents destructive operations
- **Rate limiting** on AI API calls
- **SQL injection protection** through parameterized queries
- **Schema introspection** keeps AI context aware but secure

---

##  Current Limitations

- Requires OpenAI API access (costs apply)
- Best performance with well-structured databases
- Complex analytical queries may need refinement
- No support for NoSQL databases (yet)

*Built in ~24 hours, so expect some rough edges. PRs welcome!*

---

##  Contributing

We built this during a hackathon pivot, so there's plenty of room for improvement:

1. Fork the repository
2. Create a feature branch (`git checkout -b amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin amazing-feature`)
5. Open a Pull Request

---

## 📝 License

MIT License - feel free to use this in your own projects, improve it, or just steal the good parts.

---

##  Credits

Built at **Hexafall 2025** by a team that:
- Started with a completely different idea
- Pivoted halfway through when that didn't work
- Built this instead
- Didn't win the hackathon
- Shipped something useful anyway

Sometimes the best ideas come from productive panic.

---

##  FAQ

**Q: Why "DummyDB"?**  
A: We got tired of writing dummy SQL for dummy projects. Now the AI writes it for us. We're the dummies, but smarter ones.

**Q: Is this production-ready?**  
A: It's hackathon-ready, which means it works but probably shouldn't handle your life savings.

**Q: Can I use this with my existing database?**  
A: Yes! Just point it to your database URL and start asking questions.

**Q: How much does it cost to run?**  
A: Mainly OpenAI API costs - roughly $0.01-0.05 per query depending on complexity.

---

*Ready to make your database chatty? Clone, configure, and start the conversation.*
