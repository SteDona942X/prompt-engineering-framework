# Evaluative Prompt Template

## 🎯 Purpose
Systematic evaluation of content, proposals, or data across multiple criteria with quantitative scoring and structured feedback.

## 📋 Template Structure

```markdown
**Role**: Act as a {{expert_evaluator_role}}

**Task**: Your task is to evaluate the following {{content_type}} based on these criteria:

**Evaluation Criteria**:
- {{criterion_1}} (Weight: {{weight_1}}%)
- {{criterion_2}} (Weight: {{weight_2}}%)
- {{criterion_3}} (Weight: {{weight_3}}%)

**Input**: {{content_to_evaluate}}

**Output Format**:
| Criterion | Score (1-10) | Rationale | Improvement Suggestions |
|-----------|--------------|-----------|-------------------------|
| {{criterion_1}} | X/10 | Brief explanation | Specific recommendations |
| {{criterion_2}} | X/10 | Brief explanation | Specific recommendations |
| {{criterion_3}} | X/10 | Brief explanation | Specific recommendations |

**Overall Score**: {{weighted_average}}/10
**Recommendation**: {{final_recommendation}}

**Constraints**:
- Provide specific evidence for each score
- Keep rationale to {{max_rationale_words}} words per criterion
- Include actionable improvement suggestions
- Maintain {{evaluation_tone}} throughout
```

## 🔧 Customization Variables

| Variable | Description | Example Values |
|----------|-------------|----------------|
| `{{expert_evaluator_role}}` | Evaluator expertise | "senior business analyst", "marketing strategist", "technical reviewer" |
| `{{content_type}}` | What's being evaluated | "business proposal", "marketing campaign", "technical documentation" |
| `{{criterion_1/2/3}}` | Evaluation dimensions | "feasibility", "market potential", "technical quality" |
| `{{weight_1/2/3}}` | Criterion importance | "40", "35", "25" (must sum to 100%) |
| `{{max_rationale_words}}` | Length constraint | "50", "100", "150" |
| `{{evaluation_tone}}` | Communication style | "objective", "constructive", "detailed", "executive-level" |

## 💡 Ready-to-Use Examples

### 1. Business Proposal Evaluation
```markdown
**Role**: Act as a senior investment analyst with 10+ years experience in venture capital

**Task**: Your task is to evaluate the following business proposal based on these criteria:

**Evaluation Criteria**:
- Market Viability (Weight: 40%)
- Technical Feasibility (Weight: 30%)
- Financial Projections (Weight: 30%)

**Input**: [Business proposal document or summary]

**Output Format**:
| Criterion | Score (1-10) | Rationale | Improvement Suggestions |
|-----------|--------------|-----------|-------------------------|
| Market Viability | X/10 | Market size, competition, demand evidence | Specific market research recommendations |
| Technical Feasibility | X/10 | Technology readiness, team capability | Technical development suggestions |
| Financial Projections | X/10 | Revenue model, cost structure realism | Financial modeling improvements |

**Overall Score**: {{weighted_average}}/10
**Recommendation**: APPROVE/CONDITIONAL/REJECT with specific rationale

**Constraints**:
- Provide specific evidence for each score
- Keep rationale to 100 words per criterion
- Include actionable improvement suggestions
- Maintain objective and constructive tone throughout
```

### 2. Marketing Campaign Assessment
```markdown
**Role**: Act as a digital marketing strategist specializing in B2B SaaS campaigns

**Task**: Your task is to evaluate the following marketing campaign based on these criteria:

**Evaluation Criteria**:
- Target Audience Alignment (Weight: 35%)
- Creative Quality and Messaging (Weight: 30%)
- Channel Strategy and Budget Allocation (Weight: 35%)

**Input**: [Campaign brief, creative assets, and budget breakdown]

**Output Format**:
| Criterion | Score (1-10) | Rationale | Improvement Suggestions |
|-----------|--------------|-----------|-------------------------|
| Target Audience Alignment | X/10 | Persona match, message relevance | Audience refinement recommendations |
| Creative Quality | X/10 | Visual appeal, message clarity | Creative enhancement suggestions |
| Channel Strategy | X/10 | Channel selection, budget efficiency | Optimization recommendations |

**Overall Score**: {{weighted_average}}/10
**Recommendation**: LAUNCH/REVISE/REDESIGN with specific next steps

**Constraints**:
- Provide specific evidence for each score
- Keep rationale to 75 words per criterion
- Include actionable improvement suggestions
- Maintain strategic and data-driven tone throughout
```

### 3. Technical Documentation Review
```markdown
**Role**: Act as a technical writing specialist with expertise in API documentation

**Task**: Your task is to evaluate the following technical documentation based on these criteria:

**Evaluation Criteria**:
- Clarity and Comprehensiveness (Weight: 40%)
- Technical Accuracy (Weight: 35%)
- User Experience and Navigation (Weight: 25%)

**Input**: [Documentation sections or complete technical guide]

**Output Format**:
| Criterion | Score (1-10) | Rationale | Improvement Suggestions |
|-----------|--------------|-----------|-------------------------|
| Clarity & Comprehensiveness | X/10 | Information completeness, explanation quality | Content enhancement recommendations |
| Technical Accuracy | X/10 | Code examples, procedure correctness | Technical correction suggestions |
| User Experience | X/10 | Structure, navigation, accessibility | UX improvement recommendations |

**Overall Score**: {{weighted_average}}/10
**Recommendation**: PUBLISH/REVISE/MAJOR_REVISION with priority areas

**Constraints**:
- Provide specific evidence for each score
- Keep rationale to 80 words per criterion
- Include actionable improvement suggestions
- Maintain technical and user-focused tone throughout
```

## 🎛️ Advanced Evaluation Features

### Multi-Stakeholder Perspectives
Incorporate different viewpoint evaluations:
```markdown
**Stakeholder Analysis**:
- **Executive Perspective**: Strategic alignment and ROI focus
- **Technical Perspective**: Implementation feasibility and quality
- **User Perspective**: Usability and value proposition
- **Market Perspective**: Competitive positioning and demand
```

### Confidence Scoring
Add uncertainty assessment to evaluations:
```markdown
**Confidence Levels**:
- **High Confidence (90-100%)**: Strong evidence supporting score
- **Medium Confidence (70-89%)**: Good evidence with some uncertainty
- **Low Confidence (50-69%)**: Limited evidence, requires more information
- **Insufficient Data (<50%)**: Cannot reliably evaluate this criterion
```

### Comparative Evaluation
Framework for comparing multiple options:
```markdown
**Comparative Analysis Format**:
| Criterion | Option A | Option B | Option C | Best Choice | Rationale |
|-----------|----------|----------|----------|-------------|-----------|
| {{criterion_1}} | X/10 | Y/10 | Z/10 | Option X | Specific reasons |
| {{criterion_2}} | X/10 | Y/10 | Z/10 | Option Y | Specific reasons |
| {{criterion_3}} | X/10 | Y/10 | Z/10 | Option Z | Specific reasons |
```

### Risk Assessment Integration
Include risk factors in evaluation:
```markdown
**Risk Analysis**:
- **High Risk Factors**: Elements that could significantly impact success
- **Medium Risk Factors**: Important considerations requiring monitoring
- **Low Risk Factors**: Minor concerns with manageable impact
- **Risk Mitigation**: Specific strategies to address identified risks
```

## 📊 Scoring Methodologies

### Standard 1-10 Scale
```markdown
## Score Interpretation Guide

**9-10: Exceptional**
- Exceeds expectations significantly
- Best-in-class performance
- Minimal improvement needed

**7-8: Good**
- Meets expectations well
- Strong performance with minor areas for improvement
- Recommended with small refinements

**5-6: Acceptable**
- Meets basic requirements
- Adequate performance with notable improvement opportunities
- Conditional approval with specific enhancements

**3-4: Below Standard**
- Does not meet expectations
- Significant improvement required
- Requires major revision before approval

**1-2: Poor**
- Far below expectations
- Fundamental issues requiring complete rework
- Not recommended for approval
```

### Weighted Scoring Calculation
```markdown
## Weighted Score Formula

**Step 1**: Assign individual scores (1-10) for each criterion
**Step 2**: Multiply each score by its weight percentage
**Step 3**: Sum all weighted scores for final score

**Example**:
- Criterion A: 8/10 × 40% = 3.2 points
- Criterion B: 6/10 × 35% = 2.1 points  
- Criterion C: 7/10 × 25% = 1.75 points
- **Total**: 7.05/10 overall score
```

### Industry-Specific Adaptations
```markdown
## Sector-Customized Scoring

### Technology Products
- **Innovation Factor**: Novelty and technical advancement
- **Scalability Potential**: Growth and expansion capability
- **Market Disruption**: Competitive advantage potential

### Financial Services
- **Risk Assessment**: Regulatory and market risk factors
- **Compliance Adherence**: Regulatory requirement fulfillment
- **ROI Projections**: Financial return and profitability analysis

### Healthcare Solutions
- **Patient Safety**: Risk mitigation and safety protocols
- **Clinical Efficacy**: Treatment effectiveness and outcomes
- **Regulatory Compliance**: FDA, HIPAA, and quality standards
```

## 🔒 Professional Package Features

**This basic template provides 3-criteria evaluation. Upgrade for:**

### Advanced Evaluation Systems
- **5-Dimension Framework**: Comprehensive evaluation with specialized criteria
- **Chain-of-Thought Evaluation**: Step-by-step reasoning documentation
- **Multi-Round Assessment**: Iterative evaluation with refinement cycles
- **Stakeholder Integration**: Multiple perspective synthesis

### Enhanced Analytics
- **Trend Analysis**: Performance tracking over time
- **Benchmark Comparison**: Industry standard evaluation
- **Predictive Scoring**: Success probability assessment
- **ROI Impact Modeling**: Financial outcome projections

### Team Collaboration Features
- **Reviewer Assignment**: Structured peer review workflows
- **Consensus Building**: Multi-evaluator score reconciliation
- **Audit Trails**: Complete evaluation history and reasoning
- **Template Customization**: Industry and role-specific adaptations

**Pricing**: €297 Professional Package | €997 Enterprise License

[Upgrade to Professional Package →](mailto:matteoblu1@gmail.com)

## 📈 Evaluation Quality Metrics

Track evaluation effectiveness:
- **Decision Accuracy**: Percentage of evaluations leading to successful outcomes
- **Consistency**: Score variation between evaluators for same content
- **Completeness**: Coverage of all relevant evaluation dimensions
- **Actionability**: Usefulness of improvement recommendations

## 🎯 Best Practices for Evaluators

### Preparation Guidelines
- **Understand Context**: Know the purpose and stakes of the evaluation
- **Clarify Criteria**: Ensure evaluation dimensions are well-defined
- **Gather Evidence**: Collect relevant data and supporting information
- **Set Expectations**: Establish realistic benchmarks and standards

### Evaluation Process
- **Systematic Review**: Follow consistent evaluation sequence
- **Document Evidence**: Record specific examples supporting scores
- **Consider Multiple Perspectives**: Account for different stakeholder viewpoints
- **Calibrate Scores**: Use full range of scoring scale appropriately

### Communication Excellence
- **Specific Feedback**: Provide concrete examples and evidence
- **Constructive Tone**: Focus on improvement rather than criticism
- **Actionable Recommendations**: Suggest specific, implementable improvements
- **Clear Priorities**: Highlight most important areas for enhancement

## 🤝 Feedback & Improvement

**Found this template valuable?** Help us enhance it:
- ⭐ Star the repository and share with colleagues
- 💬 Discuss your evaluation use cases in [Discussions](../../discussions)
- 🐛 Report issues or suggest criteria improvements
- 🔄 Submit your evaluation examples via Pull Request

## 📚 Related Resources

- [Instructional Prompt Template](./instructional-prompt.md) - Task-specific instructions
- [Agent Design Template](./agent-design-basic.md) - AI agent blueprints
- [6-Phase Methodology](../../docs/methodology/6-phase-framework.md) - Development process
- [Best Practices](../../docs/methodology/best-practices.md) - Quality guidelines

---

**Next Template**: [Agent Design Basic →](./agent-design-basic.md)

**Back to**: [Basic Templates Overview](./README.md)
