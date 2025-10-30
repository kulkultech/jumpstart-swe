# Repository-Wide Custom Instructions

## About This Repository

This is the **Jumpstart SWE** project - a practical e-book designed to help rising software engineering talent in Indonesia accelerate their careers. The book distills years of real-world experience into actionable advice for navigating the tech industry, especially in challenging market conditions.

**Key Context:**
- **Educational purpose only** - This is a non-commercial resource for learning
- **Target audience** - Early-career engineers, interns, and new graduates in Indonesia
- **Status** - No longer actively maintained, but contributions that improve the content are welcome

## Repository Structure

```
jumpstart-swe/
├── book/
│   ├── front-matter/       # Foreword and preface
│   └── chapters/           # Numbered chapters (00-11)
├── .github/                # GitHub configuration
│   └── copilot-instructions.md (this file)
├── AGENTS.md               # Detailed agent instructions
├── README.md               # Project overview and chapter status
├── CONTRIBUTING.md         # Contribution guidelines
├── build.sh                # Build script for generating epub
├── Makefile                # Build automation
└── cover.png               # Book cover image
```

## When Working in This Repository

### Always Check First

1. **Read AGENTS.md** - Contains detailed instructions for writing style, tone, and workflow
2. **Check README.md** - Review the chapter status table to understand what's already done
3. **Review existing chapters** - Understand the established voice and style before writing new content
4. **Read CONTRIBUTING.md** - Understand the build process and contribution workflow

### Core Principles

- **Minimal changes** - Only modify what's necessary to accomplish the task
- **Maintain consistency** - Match the existing writing style and tone
- **Update status** - Always update the chapter status table in README.md when completing work
- **Build and verify** - Run `make` to ensure the book builds successfully after changes
- **Indonesian context matters** - Keep the target audience (Indonesian rising talent) in mind

### Writing Style Requirements

When working on book content, remember:

- **Conversational tone** - Write as if speaking to a friend over coffee
- **Specific and actionable** - Avoid generic advice; provide concrete steps
- **Critical yet encouraging** - Be honest about challenges while showing paths forward
- **Story-driven** - Use real examples and anecdotes
- **Scannable format** - Short paragraphs, clear headers, bullet points

Follow the style guidelines detailed in AGENTS.md.

### Workflow for Content Changes

1. **Structure phase** - Create or review the chapter outline
2. **Writing phase** - Implement the content following AGENTS.md guidelines
3. **Update status** - Modify the status table in README.md:
   - 📋 **Planned** → 📝 **Draft** (when starting)
   - 📝 **Draft** → ✅ **Complete** (when finished)
4. **Verify build** - Run `make` to ensure the epub builds correctly
5. **Review quality** - Use the quality checklist in AGENTS.md

### Technical Guidelines

**Building the Book:**
```bash
make        # Generate the epub file
make clean  # Remove generated files
```

**Prerequisites:**
- Pandoc must be installed (see CONTRIBUTING.md)

**File Conventions:**
- Chapter files: `book/chapters/##-descriptive-name.md`
- Front matter: `book/front-matter/*.md`
- Use proper markdown formatting
- Keep line lengths reasonable for better diffs

### Important: Status Updates

**Critical Rule:** After any work on chapters, you MUST update the chapter status table in `/README.md`. This is how we track progress and avoid duplicate work.

Status meanings:
- **📋 Planned** - Structure exists, content needs writing
- **📝 Draft** - Actively being written or has initial content
- **✅ Complete** - Fully written and reviewed

### What NOT to Do

- Don't remove or modify existing working content without good reason
- Don't add build artifacts or generated files to git (they're in .gitignore)
- Don't mark chapters as complete if they need more work
- Don't ignore the Indonesian context when writing content
- Don't write in an academic or overly formal style
- Don't copy content from other sources without adding unique value
- Don't introduce technical jargon without explanation

### Code Changes

For any code or script changes:
- Follow existing patterns in `build.sh` and `Makefile`
- Test thoroughly before committing
- Keep changes minimal and focused
- Ensure backward compatibility

### Testing Your Changes

Before finalizing any content work:

1. **Build test**: Run `make` - it should complete without errors
2. **Content review**: Read your changes out loud - does it sound natural?
3. **Status check**: Verify README.md status table is updated
4. **Quality check**: Review against the checklist in AGENTS.md

### Getting Help

- **For writing style questions**: See AGENTS.md
- **For build issues**: See CONTRIBUTING.md
- **For general questions**: Create an issue on GitHub
- **For content questions**: Review similar completed chapters for examples

## Special Considerations

### Target Audience Context

Always remember this book is for:
- **Indonesian software engineers** - Consider local market conditions, companies, culture
- **Early career professionals** - New grads, interns, first 1-2 years of experience
- **Career acceleration** - People looking to make smart moves to advance faster
- **Tough market conditions** - Content should be realistic about competition and challenges

### Tone Balance

Find the right balance:
- **Authoritative but humble** - Share experience without being preachy
- **Critical but supportive** - Point out mistakes without being discouraging
- **Realistic but optimistic** - Acknowledge challenges while showing solutions
- **Professional but friendly** - Informative without being stiff

## Summary

This repository is more than just code - it's a resource that could help shape someone's career. Treat it with care:

1. **Read AGENTS.md** for comprehensive instructions
2. **Check README.md** for current chapter status
3. **Write conversationally** - as if talking to a friend
4. **Be specific and actionable** - practical advice over theory
5. **Update status** - always keep README.md current
6. **Build and verify** - ensure `make` works after changes
7. **Respect the audience** - write for Indonesian early-career engineers

When in doubt, refer to AGENTS.md or ask for clarification. Quality matters more than speed! 🚀
