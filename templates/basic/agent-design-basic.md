# Agent Design Basic Template

## 🎯 Purpose
Blueprint for creating specialized AI agents with defined roles, capabilities, and behavioral logic for automation and workflow integration.

## 📋 Template Structure

```markdown
**Agent Name**: {{agent_codename}}

**Primary Function**: {{core_responsibility}}

**Target User**: {{intended_audience}}

**Capabilities**:
- **Input Processing**: {{input_types}}
- **Output Generation**: {{output_formats}}
- **Tools Integration**: {{available_tools}}

**Behavioral Logic**:
- **Activation Conditions**: {{trigger_criteria}}
- **Decision Framework**: {{decision_process}}
- **Escalation Rules**: {{handoff_conditions}}

**Performance Parameters**:
- **Response Time**: {{time_constraints}}
- **Quality Standards**: {{success_metrics}}
- **Operating Boundaries**: {{limitation_scope}}

**Example Interaction**:
**User**: {{sample_input}}
**Agent**: {{expected_response}}
**Action**: {{system_behavior}}
```

## 🔧 Customization Variables

| Variable | Description | Example Values |
|----------|-------------|----------------|
| `{{agent_codename}}` | Agent identifier | "ContentCraft_Bot", "DataAnalyzer_AI", "SupportGenius" |
| `{{core_responsibility}}` | Primary function | "customer support automation", "content generation", "data analysis" |
| `{{intended_audience}}` | Target users | "customer service team", "marketing department", "data analysts" |
| `{{input_types}}` | Expected inputs | "text messages", "CSV files", "API requests" |
| `{{output_formats}}` | Response types | "structured JSON", "natural language", "formatted reports" |
| `{{available_tools}}` | Integration capabilities | "CRM access", "email sending", "database queries" |
| `{{trigger_criteria}}` | Activation conditions | "customer inquiry received", "data file uploaded", "scheduled time" |
| `{{decision_process}}` | Logic framework | "rule-based routing", "confidence scoring", "priority assessment" |

## 💡 Ready-to-Use Examples

### 1. Customer Support Agent
```markdown
**Agent Name**: SupportGenius_AI

**Primary Function**: Automated customer support with intelligent routing and response generation

**Target User**: Customer service representatives and end customers

**Capabilities**:
- **Input Processing**: Customer messages, chat conversations, email inquiries
- **Output Generation**: Personalized responses, escalation flags, solution recommendations
- **Tools Integration**: CRM lookup, knowledge base search, ticket creation system

**Behavioral Logic**:
- **Activation Conditions**: New customer inquiry received via any channel
- **Decision Framework**: 
  1. Classify inquiry type (technical, billing, general)
  2. Check customer history and context
  3. Generate appropriate response or escalate if complex
- **Escalation Rules**: Forward to human agent if confidence <70% or sensitive issue detected

**Performance Parameters**:
- **Response Time**: <30 seconds for standard inquiries
- **Quality Standards**: >85% customer satisfaction score
- **Operating Boundaries**: Handle routine inquiries, escalate complex/sensitive issues

**Example Interaction**:
**User**: "My account seems to be locked and I can't access my dashboard"
**Agent**: "I understand you're having trouble accessing your dashboard. Let me check your account status... I can see there was a security lockout due to multiple login attempts. I've unlocked your account and sent a password reset link to your email. You should be able to access your dashboard in 2-3 minutes. Is there anything else I can help you with?"
**Action**: Account unlocked, password reset triggered, satisfaction survey scheduled
```

### 2. Content Generation Agent
```markdown
**Agent Name**: ContentCraft_Pro

**Primary Function**: Automated content creation for marketing campaigns and social media

**Target User**: Marketing team members and content creators

**Capabilities**:
- **Input Processing**: Content briefs, brand guidelines, target audience data
- **Output Generation**: Blog posts, social media content, email campaigns, ad copy
- **Tools Integration**: Brand asset library, publishing calendar, analytics tools

**Behavioral Logic**:
- **Activation Conditions**: Content request submitted with complete brief
- **Decision Framework**:
  1. Analyze content requirements and objectives
  2. Select appropriate tone and format based on audience
  3. Generate content following brand guidelines
  4. Include relevant CTAs and optimization elements
- **Escalation Rules**: Request human review for sensitive topics or high-stakes campaigns

**Performance Parameters**:
- **Response Time**: <15 minutes for standard content pieces
- **Quality Standards**: Brand compliance >95%, engagement rate >industry average
- **Operating Boundaries**: Create marketing content, avoid legal/medical claims

**Example Interaction**:
**User**: "Create 5 LinkedIn posts for our new AI productivity tool launch, targeting startup founders"
**Agent**: "I'll create 5 LinkedIn posts for your AI productivity tool launch targeting startup founders. Here's your content calendar:

Post 1: Problem/Solution Hook - 'Founders: Spending 60% of your time on admin tasks?'
Post 2: Feature Spotlight - 'How our AI handles your routine workflows automatically'
Post 3: Social Proof - 'Join 500+ startups already saving 20 hours/week'
Post 4: Behind-the-Scenes - 'Why we built this tool (founder story)'
Post 5: Launch CTA - 'Limited-time founder pricing available now'

Each post includes optimal hashtags, posting times, and engagement CTAs. Would you like me to adjust the tone or focus on specific features?"
**Action**: Content generated, publishing schedule created, performance tracking enabled
```

### 3. Data Analysis Agent
```markdown
**Agent Name**: InsightEngine_AI

**Primary Function**: Automated data analysis and business intelligence reporting

**Target User**: Business analysts, managers, and data teams

**Capabilities**:
- **Input Processing**: CSV files, database queries, spreadsheet data
- **Output Generation**: Executive summaries, trend analysis, predictive insights
- **Tools Integration**: BI tools, databases, visualization platforms

**Behavioral Logic**:
- **Activation Conditions**: New data file uploaded or analysis request submitted
- **Decision Framework**:
  1. Validate data quality and completeness
  2. Identify relevant analysis methods based on data type
  3. Generate insights with confidence indicators
  4. Create visualizations and executive summary
- **Escalation Rules**: Flag data quality issues, request clarification for ambiguous requirements

**Performance Parameters**:
- **Response Time**: <5 minutes for standard datasets (<10k rows)
- **Quality Standards**: >90% accuracy on key metrics, actionable insights in 100% of reports
- **Operating Boundaries**: Analyze structured data, avoid sensitive personal information

**Example Interaction**:
**User**: "Analyze Q3 sales performance by region and identify growth opportunities"
**Agent**: "Analysis of Q3 sales data complete. Key findings:

📊 **Performance Summary:**
- Total Q3 Revenue: $2.4M (+15% vs Q2)
- Top Region: West Coast (40% of revenue)
- Fastest Growth: Southeast (+28% vs Q2)

🎯 **Growth Opportunities:**
1. **Southeast Expansion**: 28% growth rate suggests untapped potential
2. **Product Mix Optimization**: Premium products show 45% higher margins
3. **Seasonal Targeting**: August showed 35% spike in enterprise sales

📈 **Recommendations:**
- Increase Southeast sales team by 2 reps (projected +$180k revenue)
- Launch premium product campaign in top 3 regions
- Develop Q4 enterprise outreach strategy

Confidence Level: 92% (based on 3-year historical data)
Would you like me to dive deeper into any specific region or create a detailed action plan?"
**Action**: Report generated, visualizations created, follow-up analysis queued
```

## 🎛️ Advanced Agent Features

### Multi-Modal Capabilities
Enhance agents with diverse input/output handling:
```markdown
**Advanced Input Processing**:
- **Text Analysis**: Natural language understanding and intent recognition
- **File Processing**: Document parsing, data extraction, format conversion
- **API Integration**: Real-time data fetching and system connectivity
- **Voice Commands**: Speech-to-text processing and voice response generation

**Enhanced Output Generation**:
- **Dynamic Formatting**: Adaptive presentation based on user preferences
- **Multi-Channel Distribution**: Simultaneous delivery across platforms
- **Interactive Elements**: Clickable buttons, forms, and decision trees
- **Multimedia Integration**: Charts, images, and rich media inclusion
```

### Learning and Adaptation
Build agents that improve over time:
```markdown
**Performance Learning**:
- **Success Pattern Recognition**: Identify what works best for different scenarios
- **User Preference Adaptation**: Customize responses based on individual user history
- **Context Awareness**: Improve responses using conversation and historical context
- **Feedback Integration**: Incorporate user ratings and corrections into future responses

**Continuous Optimization**:
- **A/B Testing**: Compare different response strategies automatically
- **Performance Monitoring**: Track key metrics and identify improvement opportunities
- **Model Updates**: Integrate new capabilities and knowledge as available
- **Quality Assurance**: Maintain consistency while enabling adaptive improvements
```

### Team Collaboration
Design agents for multi-user environments:
```markdown
**Collaboration Features**:
- **Shared Context**: Maintain awareness of team conversations and decisions
- **Role-Based Access**: Different capabilities and information access by user role
- **Workflow Integration**: Connect with existing team tools and processes
- **Knowledge Sharing**: Learn from all team interactions and share insights

**Coordination Mechanisms**:
- **Task Handoffs**: Smooth transitions between agents and human team members
- **Status Updates**: Keep relevant stakeholders informed of progress and decisions
- **Resource Management**: Coordinate access to shared tools and information
- **Conflict Resolution**: Handle competing requests and priority conflicts gracefully
```

## 🔧 Implementation Patterns

### Deployment Strategies

#### **Standalone Agent**
```markdown
## Independent Operation Model

**Use Cases**: Simple, well-defined tasks with clear boundaries
**Benefits**: Easy to implement, test, and maintain
**Limitations**: Cannot handle complex workflows requiring multiple capabilities

**Implementation Approach**:
1. Define single, focused responsibility
2. Create comprehensive input validation
3. Implement robust error handling
4. Establish clear escalation criteria
5. Monitor performance and user satisfaction
```

#### **Agent Team Coordination**
```markdown
## Multi-Agent Orchestration

**Use Cases**: Complex workflows requiring specialized capabilities
**Benefits**: Scalable, maintainable, allows for specialized expertise
**Limitations**: Requires coordination logic and handoff protocols

**Implementation Approach**:
1. Design agent specializations and responsibilities
2. Create communication protocols between agents
3. Implement workflow orchestration logic
4. Establish shared context and state management
5. Monitor overall system performance and coordination effectiveness
```

#### **Human-Agent Hybrid**
```markdown
## Collaborative Operation Model

**Use Cases**: Tasks requiring both AI efficiency and human judgment
**Benefits**: Combines automation benefits with human oversight
**Limitations**: Requires careful coordination and clear role definitions

**Implementation Approach**:
1. Define clear boundaries between agent and human responsibilities
2. Create seamless handoff mechanisms
3. Implement context preservation during transitions
4. Establish quality assurance and feedback loops
5. Monitor collaboration effectiveness and user satisfaction
```

### Integration Patterns

#### **API-First Design**
```markdown
## System Integration Strategy

**Connectivity Requirements**:
- RESTful API endpoints for external system communication
- Webhook support for real-time event processing
- Authentication and authorization for secure access
- Rate limiting and error handling for robust operation

**Data Exchange Formats**:
- JSON for structured data communication
- File upload/download for document processing
- Real-time messaging for interactive conversations
- Batch processing for high-volume operations
```

#### **Workflow Automation**
```markdown
## Process Integration Framework

**Automation Platforms**:
- n8n workflow integration for complex process automation
- Zapier connectivity for simple trigger-action workflows
- Custom API development for specialized integration needs
- Database connectivity for data persistence and retrieval

**Event-Driven Architecture**:
- Trigger-based activation for responsive operation
- Queue management for high-volume processing
- Asynchronous processing for complex or time-consuming tasks
- Real-time monitoring and alerting for operational awareness
```

## 🔒 Professional Package Features

**This basic template provides single-agent design. Upgrade for:**

### Enterprise Agent Architecture
- **Multi-Agent Orchestration**: Coordinated team of specialized agents
- **Advanced Learning Systems**: Continuous improvement and adaptation
- **Enterprise Integration**: Deep connectivity with business systems
- **Compliance Framework**: Regulatory adherence and audit capabilities

### Advanced Capabilities
- **Natural Language Processing**: Sophisticated conversation management
- **Predictive Analytics**: Proactive insights and recommendation generation
- **Workflow Optimization**: Dynamic process improvement and automation
- **Security Framework**: Advanced authentication, authorization, and data protection

### Management and Monitoring
- **Performance Analytics**: Comprehensive metrics and optimization insights
- **Team Collaboration**: Multi-user agent development and management
- **Version Control**: Agent evolution tracking and rollback capabilities
- **Enterprise Support**: Professional implementation and ongoing optimization

**Pricing**: €297 Professional Package | €997 Enterprise License

[Upgrade to Professional Package →](mailto:matteoblu1@gmail.com)

## 📊 Agent Performance Metrics

Track agent effectiveness:
- **Task Completion Rate**: Percentage of requests successfully handled without escalation
- **Response Quality**: User satisfaction scores and feedback ratings
- **Efficiency Gains**: Time savings compared to manual processes
- **Learning Progress**: Improvement in performance metrics over time

## 🛡️ Security and Compliance

### Data Protection
- **Input Sanitization**: Validate and clean all incoming data
- **Output Filtering**: Ensure responses don't contain sensitive information
- **Access Control**: Implement role-based permissions and authentication
- **Audit Logging**: Maintain comprehensive records of agent interactions

### Operational Safety
- **Boundary Enforcement**: Prevent agents from exceeding authorized capabilities
- **Error Handling**: Graceful degradation and informative error messages
- **Escalation Protocols**: Clear procedures for handling complex or sensitive situations
- **Performance Monitoring**: Real-time tracking of agent behavior and performance

## 🤝 Feedback & Improvement

**Found this template helpful?** Contribute to its evolution:
- ⭐ Star the repository and share with your team
- 💬 Discuss your agent implementations in [Discussions](../../discussions)
- 🐛 Report issues or suggest capability enhancements
- 🔄 Submit your agent examples and use cases via Pull Request

## 📚 Related Resources

- [Instructional Prompt Template](./instructional-prompt.md) - Task-specific instructions
- [Evaluative Prompt Template](./evaluative-prompt.md) - Multi-criteria assessment
- [6-Phase Methodology](../../docs/methodology/6-phase-framework.md) - Development process
- [Case Studies](../../docs/case-studies/README.md) - Real-world implementations

---

**Next Template**: [Meta-Prompt Starter →](./meta-prompt-starter.md)

**Back to**: [Basic Templates Overview](./README.md)
