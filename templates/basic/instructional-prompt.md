# Instructional Prompt Template

## 🎯 Purpose
Provide clear, structured instructions to LLMs for consistent task execution with defined output formats.

## 📋 Template Structure

```markdown
**Role**: Act as {{expert_role}}

**Task**: Your task is to {{task_description}}

**Input Expected**: {{input_description}}

**Output Format**: {{output_format}}

**Constraints**:
- Maximum {{max_words}} words
- Avoid {{undesired_behavior}}
- Tone: {{tone_style}}
- Include {{required_elements}}

**Example**:
{{example_input}} → {{example_output}}
```

## 🔧 Customization Variables

| Variable | Description | Example Values |
|----------|-------------|----------------|
| `{{expert_role}}` | Professional persona | "senior data analyst", "marketing strategist", "technical writer" |
| `{{task_description}}` | Specific task | "analyze quarterly sales data", "create social media content" |
| `{{input_description}}` | Expected input type | "CSV file with sales data", "product specifications" |
| `{{output_format}}` | Desired output structure | "JSON with metrics", "bullet-point summary", "executive report" |
| `{{max_words}}` | Length constraint | "500", "1000", "no limit" |
| `{{undesired_behavior}}` | What to avoid | "speculation", "personal opinions", "technical jargon" |
| `{{tone_style}}` | Communication style | "professional", "casual", "technical", "persuasive" |
| `{{required_elements}}` | Must-include items | "data sources", "confidence levels", "recommendations" |

## 💡 Ready-to-Use Examples

### 1. Content Creation
```markdown
**Role**: Act as a content marketing specialist

**Task**: Your task is to create an editorial calendar for LinkedIn

**Input Expected**: Business sector, target audience, marketing objectives

**Output Format**: Table with 10 post ideas, each with headline, main content, CTA

**Constraints**:
- Maximum 2000 characters per post
- Avoid direct promotional content
- Tone: professional but engaging
- Include at least 3 posts with case studies

**Example**:
Input: "B2B SaaS, target: startup founders, objective: lead generation"
Output: [Structured table with post ideas]
```

### 2. Data Analysis
```markdown
**Role**: Act as a senior business analyst

**Task**: Your task is to analyze quarterly sales performance

**Input Expected**: CSV file with sales data by product, region, and month

**Output Format**: Executive summary with key insights, identified trends, actionable recommendations

**Constraints**:
- Maximum 800 words
- Avoid speculation not supported by data
- Tone: objective and data-driven
- Include confidence levels for each insight

**Example**:
Input: [Sales_Q3_2024.csv with columns: Product, Region, Month, Revenue, Units]
Output: "Executive Summary: Q3 Performance Analysis..."
```

### 3. Process Documentation
```markdown
**Role**: Act as a technical writer specializing in business processes

**Task**: Your task is to document an operational process

**Input Expected**: Informal process description, stakeholders involved, tools used

**Output Format**: Structured document with numbered steps, responsibilities, checkpoints

**Constraints**:
- Maximum 1500 words
- Avoid procedural ambiguities
- Tone: clear and instructional
- Include text-based flow diagrams

**Example**:
Input: "How we handle customer support requests via email"
Output: [Structured step-by-step process]
```

## 🎛️ Advanced Customization

### Error Handling
Add fallback instructions for edge cases:
```markdown
**Fallback Instructions**:
- If input data is incomplete: Request specific missing information
- If task scope is unclear: Ask clarifying questions before proceeding
- If output format cannot be achieved: Provide closest alternative with explanation
```

### Quality Control
Include validation criteria:
```markdown
**Quality Checklist**:
- [ ] All required elements included
- [ ] Output format matches specification
- [ ] Tone is consistent throughout
- [ ] No undesired behaviors present
- [ ] Example provided if requested
```

## 🔒 Professional Package Features

**This basic template provides essential functionality. Upgrade for:**

### Advanced Features
- **Multi-Model Optimization**: Specific adaptations for GPT-4, Claude, Gemini
- **Dynamic Parameter Adjustment**: Context-sensitive variable modification
- **Performance Monitoring**: Built-in metrics for consistency tracking
- **Team Collaboration**: Version control and shared template libraries

### Enhanced Templates
- **Conditional Logic**: If-then instructions for complex scenarios
- **Chain-of-Thought Integration**: Step-by-step reasoning frameworks
- **Error Recovery**: Automated fallback and retry mechanisms
- **API Integration**: Direct connection to workflow automation tools

**Pricing**: €297 Professional Package | €997 Enterprise License

[Upgrade to Professional Package →](mailto:matteoblu1@gmail.com)

## 📊 Success Metrics

Track template effectiveness:
- **Consistency**: Same input produces similar outputs (target: >85%)
- **Completeness**: All required elements included (target: 100%)
- **Efficiency**: Reduces prompt iteration cycles (target: 60% reduction)
- **Adoption**: Team usage and satisfaction scores

## 🤝 Feedback & Improvement

**Found this template useful?** Help us improve:
- ⭐ Star the repository
- 💬 Share your use case in [Discussions](../../discussions)
- 🐛 Report issues or suggest improvements
- 🔄 Submit your own example via Pull Request

## 📚 Related Resources

- [Evaluative Prompt Template](./evaluative-prompt.md) - Multi-criteria assessment
- [Agent Design Template](./agent-design-basic.md) - AI agent blueprints  
- [6-Phase Methodology](../../docs/methodology/6-phase-framework.md) - Complete development process
- [Quick Start Guide](../../docs/quick-start.md) - Implementation basics

---

**Next Template**: [Evaluative Prompt →](./evaluative-prompt.md)

**Back to**: [Basic Templates Overview](./README.md)
