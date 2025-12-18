# Seemse AI Admin

> English Documentation | [中文文档](./README.md)

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![GitHub Stars](https://img.shields.io/github/stars/seemse/seemse-ai-admin.svg?style=social)
![GitHub Forks](https://img.shields.io/github/forks/seemse/seemse-ai-admin.svg?style=social)
![Based on RuoYi-AI](https://img.shields.io/badge/Based%20on-RuoYi--AI-blue.svg)

An **enterprise-grade AI management backend system deeply customized based on RuoYi-AI**, inheriting the high availability and extensibility of the RuoYi ecosystem, focusing on "AI capability management + enterprise-grade permission control" core scenarios. It solves pain points such as complex AI system management, chaotic permissions, and difficult deployment, achieving a balance between rapid AI capability access and efficient management.

## 🔗 Project Origin

This project is developed based on [RuoYi-AI](https://github.com/ageerle/ruoyi-ai) (RuoYi AI Enhanced Edition), retaining the core capabilities of the RuoYi framework such as **permission management, system configuration, and user management**, while deeply customizing for "AI application scenarios":

* Expanding exclusive modules for "AI model management, digital human configuration, knowledge base management"
* Strengthening core functions of "refined permission grading and AI resource security control"
* Integrating AI capabilities of "multi-model access, intelligent dialogue, data analysis"
* Adapting to enterprise needs of "enterprise-level AI deployment, multi-tenant management, compliance auditing"

> Thanks to the RuoYi-AI team for providing the excellent foundational framework. This project will continue to synchronize stability updates and security patches from the upstream framework.

## 🌐 Project Ecosystem

Seemse AI is a complete artificial intelligence solution that includes the following core projects:

### 📦 Core Projects
- **Backend Project** : [https://github.com/seemse/seemse_ai](https://github.com/seemse/seemse_ai) 
  - AI service backend built with Spring Boot + MyBatis Plus
  - Provides core API services for user management, AI model management, conversation processing
  - Supports multiple AI model integrations (OpenAI, Claude, Wenxin Yiyan, etc.)

- **Admin Panel** : [https://github.com/seemse/seemse-ai-admin](https://github.com/seemse/seemse-ai-admin)  
  - Enterprise-level admin backend based on Vue 3 + Ant Design Vue
  - Provides user management, system configuration, AI model configuration, data statistics
  - Supports enterprise features like permission management, system monitoring, log management

- **Chat Application Frontend** : [https://github.com/seemse/seemse-ai-web](https://github.com/seemse/seemse-ai-web)
  - Modern chat application based on Vue 3 + TypeScript
  - Supports multi-model conversations, history records, file uploads
  - Responsive design supporting PC and mobile access

### 🔗 Project Relationship Diagram
```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│  seemse-ai-web  │    │ seemse-ai-admin │    │  seemse_ai      │
│  (Chat Frontend)│    │  (Admin Panel)  │    │  (Backend)      │
└─────────────────┘    └─────────────────┘    └─────────────────┘
         │                       │                       │
         └───────────────────────┼───────────────────────┘
                                 │
                    ┌─────────────────┐
                    │   Users/Admins  │
                    │ (Unified User   │
                    │   System)       │
                    └─────────────────┘
```

### 🎯 Quick Navigation
| Project | Tech Stack | Main Features | Status |
|---------|------------|---------------|--------|
| seemse_ai | Spring Boot, MyBatis Plus, Redis | AI Services, User Management, Model Management | ✅ Stable |
| seemse-ai-admin | Vue 3, TypeScript, Ant Design Vue | Admin Panel, System Configuration | ✅ Stable |
| seemse-ai-web | Vue 3, TypeScript, Vite | Chat Application, AI Conversations | ✅ Stable |

## 🌟 Core Features (Enhanced based on RuoYi-AI)

### 1. Unified AI Capability Management (Core Enhancement)
* **Multi-Model Support**: Unified configuration management for OpenAI, Claude, Wenxin Yiyan, Tongyi Qianwen and other AI models
* **Intelligent Routing**: Smart allocation of AI model requests based on load balancing and cost optimization strategies
* **Model Monitoring**: Real-time monitoring of model call status, response time, cost consumption and other key metrics
* **Elastic Expansion**: Support for custom model access with standardized API interface specifications

### 2. Enterprise-Grade Permission Control (Deep Optimization)
* **Fine-grained Permissions**: Based on RuoYi permission system, extended exclusive resource permissions for "AI models/knowledge base/digital humans"
* **Multi-tenant Isolation**: Support for enterprise-level multi-tenant architecture with complete data isolation, meeting SaaS deployment needs
* **Dynamic Permissions**: Support for temporary authorization, automatic recovery, permission inheritance and other advanced permission management functions
* **Security Audit**: Complete recording of AI resource access logs, supporting compliance auditing and risk warning

### 3. AI Digital Human Management (New Module)
* **Image Customization**: Support for multi-dimensional personalized configuration of digital human appearance, voice, and personality
* **Knowledge Base Association**: Intelligent binding of digital humans with knowledge bases, providing professional domain Q&A capabilities
* **Multi-scenario Adaptation**: Support for rapid deployment in various business scenarios such as customer service, education, and consulting
* **Interaction Optimization**: Continuous optimization of digital human interaction experience based on user feedback

### 4. Intelligent Knowledge Base System (New Feature)
* **Knowledge Management**: Unified management of multi-format knowledge content including documents, images, and videos
* **AI Search**: Integrated semantic understanding capabilities, supporting intelligent Q&A and knowledge recommendation
* **Permission Control**: Fine-grained knowledge access permissions, supporting department-level and project-level knowledge isolation
* **Version Management**: Knowledge content version control, supporting historical traceability and change auditing

### 5. Data Analysis and Monitoring (Inherited Enhancement)
* **Usage Statistics**: AI model call statistics, user behavior analysis, cost accounting reports
* **Performance Monitoring**: Real-time monitoring of system performance with custom alarm rules
* **Business Insights**: Business trend analysis and optimization suggestions based on AI usage data
* **Operational Support**: Provide operational data dashboards for decision analysis

### 6. Inherited RuoYi-AI Core Advantages
* **Complete Permission System**: User/role/menu permission management, ready to use out of the box
* **Front-end and Back-end Separation**: Modern architecture, easy for secondary development and function expansion
* **Enterprise Features**: Support for Docker deployment, distributed caching, load balancing
* **Development Efficiency**: Built-in code generator, supporting rapid business function development

## 📋 Applicable Scenarios

- **Enterprise AI Platform**: Unified management of AI model resources within the enterprise, providing standardized AI service interfaces
- **Intelligent Customer Service**: Deploy AI digital humans to provide 24/7 intelligent customer service support
- **Knowledge Management**: Build an enterprise knowledge base system to achieve intelligent knowledge management and sharing
- **Data Analysis Platform**: Utilize AI capabilities for intelligent analysis and prediction of enterprise data
- **Education and Training**: Provide personalized AI teaching assistants and intelligent Q&A services
- **Business Decision Support**: Provide intelligent analysis and recommendations to assist enterprise business decisions

## 🚀 Tech Stack (Extended based on RuoYi-AI)

| Module | Technology Selection | Description | AI Management Extension |
|--------|-------------------|-------------|----------------------|
| **Frontend Framework** | Vue 3 + TypeScript | Progressive JavaScript framework | Enhanced AI component library |
| **Build Tool** | Vite | Next-generation frontend build tool | AI resource optimization packaging |
| **UI Component Library** | Ant Design Vue | Enterprise-class UI component library | AI theme adaptation |
| **State Management** | Pinia | Vue state management library | AI state management |
| **Backend Framework** | Spring Boot | Microservices framework | AI service integration |
| **Security Framework** | Spring Security | Security framework | AI permission control |
| **Data Persistence** | MyBatis Plus | Data persistence framework | AI data model management |
| **Cache** | Redis | Distributed cache | AI model cache |
| **Database** | MySQL | Relational database | AI knowledge base storage |
| **API Documentation** | Knife4j | API documentation | AI interface documentation |
| **Development Tools** | Node.js + pnpm | JavaScript runtime and package manager | AI development tools |

## 🔍 Differences from RuoYi-AI

| Function | RuoYi-AI | This Project (Enhanced Version) | Advantage Description |
|----------|----------|-------------------------------|---------------------|
| **AI Model Management** | Basic model configuration | Unified management of multi-model + intelligent routing | More comprehensive model management |
| **Permission Control** | Basic RBAC permissions | Fine-grained AI resource permissions + multi-tenant isolation | More secure permission management |
| **Digital Human Function** | Not supported | Complete digital human management system | New core features |
| **Knowledge Base System** | Basic file management | Intelligent knowledge base + AI search | More intelligent knowledge management |
| **Data Analysis** | Basic statistics | AI usage analysis + business insights | More in-depth data analysis |
| **Enterprise Features** | Single-tenant architecture | Multi-tenant architecture + SaaS support | Better enterprise deployment |

## 📋 Requirements (Consistent with RuoYi-AI)

### Frontend Environment
- **Node.js**: >= 16.0.0 (Recommended: 18.x LTS)
- **pnpm**: >= 8.0.0 (Recommended: latest version)
- **Git**: >= 2.20.0
- **Browser**: Chrome >= 80, Firefox >= 75, Safari >= 13, Edge >= 80

### Backend Environment
- **Java**: >= 11 (Recommended: OpenJDK 17)
- **Spring Boot**: 2.7.x (Compatible with RuoYi-AI)
- **MySQL**: >= 8.0 (Recommended: 8.0.33+)
- **Redis**: >= 6.0 (Recommended: 7.0+)

### Development Tools
- **IDE**: VS Code (with recommended extensions) or WebStorm
- **Build Tool**: Maven >= 3.6
- **Container**: Docker >= 20.0 (Optional)

## 🚀 Quick Start

### Installation and Deployment

#### 1. Clone the Repository

```bash
# Clone the frontend project
git clone https://github.com/your-username/seemse-ai-admin.git
cd seemse-ai-admin

# Clone the backend project (required)
git clone https://github.com/your-username/seemse-ai-backend.git
```

#### 2. Environment Configuration

**Frontend Configuration:**
```bash
# Copy environment configuration file
cp .env.example .env

# Edit .env file, configure the following key parameters:
# VITE_API_URL = Backend service address (e.g., http://localhost:8080)
# VITE_APP_TITLE = System title (e.g., AI Management Platform)
# VITE_AI_MODELS = Supported AI model list
```

**Backend Configuration:**
```bash
# Enter the backend project directory
cd seemse-ai-backend

# Copy configuration file
cp src/main/resources/application.yml.example src/main/resources/application.yml

# Configure database connection, Redis connection, AI model API Key, etc.
```

#### 3. Install Dependencies

**Frontend Dependencies:**
```bash
# Install frontend dependencies
pnpm install

# Verify installation is successful
pnpm --version
```

**Backend Dependencies:**
```bash
# Enter the backend project directory
cd seemse-ai-backend

# Install Maven dependencies
mvn clean install

# Verify installation is successful
mvn -version
```

#### 4. Start Services

**Start Backend Service:**
```bash
# Enter the backend project directory
cd seemse-ai-backend

# Start the backend service (development mode)
mvn spring-boot:run

# Or use the packaged method
mvn clean package
java -jar target/seemse-ai-backend.jar
```

**Start Frontend Service:**
```bash
# Enter the frontend project directory
cd seemse-ai-admin

# Start the development server
pnpm dev

# Or use the preview mode
pnpm preview
```

#### 5. Access the System

- Frontend Address: `http://localhost:3000`
- Backend Address: `http://localhost:8080`
- API Documentation: `http://localhost:8080/swagger-ui.html`

**Default Account:**
- Username: `admin`
- Password: `admin123`

#### 6. Build Production Version

**Build Frontend:**
```bash
# Build production version
pnpm build

# Build result output to dist/ directory
# Can be deployed to Nginx, Apache and other web servers
```

**Build Backend:**
```bash
# Enter the backend project directory
cd seemse-ai-backend

# Package production version
mvn clean package -P prod

# Build result output to target/ directory
# Can be deployed to servers using java -jar
```

## 📖 Usage Guide

### Core Operation Process

#### 1. AI Model Configuration Management
1. **Model Access**: Enter the AI model management page, click "Add Model"
2. **Parameter Configuration**: Fill in model name, API Key, request address, and other parameters
3. **Permission Assignment**: Assign model usage permissions to specific roles or users
4. **Testing Verification**: Test the model connection to ensure normal access
5. **Monitoring Management**: View model call logs and performance monitoring data

#### 2. Digital Human Creation and Configuration
1. **Create Digital Human**: Enter the digital human management module, click "Create Digital Human"
2. **Basic Configuration**: Set digital human name, avatar, voice, and other basic information
3. **Knowledge Association**: Bind relevant knowledge bases to enhance professional capabilities
4. **Permission Settings**: Configure digital human usage permissions and visible range
5. **Publish Application**: Publish the digital human to specific business scenarios

#### 3. Knowledge Base Management
1. **Create Knowledge Base**: Create a knowledge base and set access permissions
2. **Upload Documents**: Support uploading documents in multiple formats (PDF, Word, Excel, etc.)
3. **Knowledge Classification**: Categorize and tag knowledge content
4. **AI Training**: Use AI technology to train and optimize knowledge bases
5. **Application Integration**: Integrate knowledge bases into digital humans or other applications

### Extension Development Path (Based on RuoYi-AI Architecture)

#### 🎯 Frontend Extension Modules (Based on RuoYi-AI View Architecture)
* **AI Capability Management Module**:
  * AI Model Management: Multi-model configuration, parameter tuning, permission control
  * Digital Human Management: Avatar configuration, knowledge base association, interaction parameter settings
  * Intelligent Dialogue: Streaming response support, multi-round dialogue, context memory

* **Knowledge Base Management Module**:
  * Knowledge Classification: Multi-level classification management, permission inheritance, visual display
  * Knowledge Documents: Multi-format support, version management, collaborative editing
  * Intelligent Retrieval: Full-text search, AI semantic matching, personalized recommendations

* **System Monitoring Module**:
  * AI Call Monitoring: Model usage rate, response time, error rate statistics
  * Resource Monitoring: Knowledge base capacity, user activity, system performance
  * Log Audit: Operation records, exception tracking, compliance reporting

* **User Permission Module**:
  * Role Management: Role permission configuration based on organizational structure
  * User Configuration: Personalized settings, usage preferences, permission inheritance
  * Organizational Structure: Department management, hierarchical relationships, permission transfer

#### 🔧 Technical Extension Points (Integration with RuoYi-AI Architecture)
* **Component Library Extension**:
  * AI Business Components: Model selector, digital human display, knowledge graph
  * Common Business Components: Permission tree, organizational chart, rich text editor
  * Visualization Components: Chart display, data dashboard, real-time monitoring

* **State Management Extension**:
  * AI Module State: Model configuration, dialogue history, knowledge base cache
  * User State: Permission information, personalized configuration, usage records
  * System State: Monitoring data, alarm information, operational indicators

* **Utility Functions Extension**:
  * AI Business Tools: Model call encapsulation, data processing, format conversion
  * Permission Tools: Permission calculation, role judgment, resource verification
  * Business Tools: Form validation, data formatting, file processing

#### 🔗 Backend Integration Instructions (Maintain Existing Backend Architecture)
* **Service Integration**: Cooperate with [seemse_ai](https://github.com/seemse/seemse_ai) backend project
* **Interface Specification**: Provide complete RESTful API interfaces, support standard HTTP methods
* **Real-time Communication**: Support WebSocket real-time communication, achieve digital human streaming response
* **Data Synchronization**: Support real-time data synchronization between frontend and backend, ensure consistency
* **Security Mechanism**: Inherit RuoYi-AI security framework, including authentication, authorization, encryption, etc.

## 🔒 Security and Compliance Guarantee (Deep Optimization)

### Data Security Guarantee
- **Data Encryption**: Use AES-256 encryption algorithm to encrypt sensitive data
- **Access Control**: Implement multi-level access control based on RBAC permission model
- **Data Isolation**: Support multi-tenant data isolation to ensure data security
- **Backup Recovery**: Provide regular data backup and quick recovery functions

### AI Content Security
- **Content Filtering**: Built-in sensitive word filtering to ensure AI output content is compliant
- **Audit Logs**: Record AI generation content completely for compliance auditing
- **Permission Control**: Fine-grained AI function permission control
- **Usage Monitoring**: Monitor AI usage to prevent abuse

### Enterprise Deployment Security
- **Network Security**: Support HTTPS encrypted transmission and network isolation
- **Identity Authentication**: Integrate enterprise SSO single sign-on system
- **Security Audit**: Provide complete security audit logs and reports
- **Compliance Standards**: Comply with GDPR, SOX and other compliance requirements

## 💻 Development Best Practices

### Development Environment Configuration
- **Node Version Management**: It is recommended to use nvm to manage Node.js versions
- **Code Editor**: It is recommended to use VS Code and install recommended extensions
- **Git Configuration**: Configure Git user information and commit message specifications
- **Development Tools**: Install necessary development tools and dependency packages

### Performance Optimization Suggestions
- **Code Splitting**: Use dynamic import for code splitting to reduce initial loading time
- **Image Optimization**: Compress images and use modern formats (WebP) to improve loading speed
- **Cache Strategy**: Configure appropriate browser caching and CDN acceleration
- **Monitoring Tools**: Use performance monitoring tools to identify and optimize performance bottlenecks

### Security Development Standards
- **Dependency Management**: Regularly update dependencies and fix security vulnerabilities
- **Code Audit**: Conduct code security audits to prevent common security issues
- **Input Validation**: Strictly validate and filter all user inputs
- **Error Handling**: Properly handle errors to avoid exposing sensitive information

### Operation and Maintenance Monitoring
- **Log Management**: Configure log collection and analysis systems
- **Performance Monitoring**: Monitor system performance metrics and set up alarms
- **Health Checks**: Configure system health checks and automatic recovery
- **Backup Strategy**: Develop data backup strategies and regularly test recovery processes

## 📚 Project Structure

```
seemse-ai-admin/                           # AI Management Platform Frontend Project
├── apps/                                   # Application directory
│   ├── web-antd/                          # Ant Design Vue version main application
│   │   ├── src/                           # Source code directory
│   │   │   ├── components/                # Business components
│   │   │   │   ├── ai/                    # AI-related components
│   │   │   │   │   ├── model-manager/     # AI model management components
│   │   │   │   │   ├── digital-human/     # Digital human management components
│   │   │   │   │   └── knowledge-base/    # Knowledge base components
│   │   │   │   ├── auth/                  # Permission-related components
│   │   │   │   └── common/                # Common components
│   │   │   ├── views/                     # Page views
│   │   │   │   ├── ai/                    # AI functional pages
│   │   │   │   ├── system/                # System management pages
│   │   │   │   └── dashboard/             # Dashboard pages
│   │   │   ├── api/                       # API interfaces
│   │   │   ├── store/                     # State management
│   │   │   ├── router/                    # Routing configuration
│   │   │   └── utils/                     # Utility functions
│   │   ├── package.json                   # Application dependencies
│   │   └── vite.config.ts                 # Vite configuration
│   └── web-ele/                           # Element Plus version (optional)
├── packages/                               # Shared packages
│   ├── ui/                                # UI component library
│   │   ├── components/                    # Basic components
│   │   ├── ai/                            # AI-specific components
│   │   └── hooks/                         # Reusable hooks
│   ├── utils/                             # Utility functions
│   │   ├── ai/                            # AI-related utilities
│   │   ├── auth/                          # Permission utilities
│   │   └── request/                       # Request utilities
│   ├── types/                             # TypeScript type definitions
│   │   ├── ai.d.ts                        # AI-related types
│   │   ├── auth.d.ts                      # Permission types
│   │   └── system.d.ts                    # System types
│   ├── api/                               # API interface definitions
│   │   ├── ai.ts                          # AI-related APIs
│   │   ├── auth.ts                        # Permission APIs
│   │   └── system.ts                      # System APIs
│   └── constants/                         # Constants definition
│       ├── ai.ts                          # AI-related constants
│       └── permissions.ts                 # Permission constants
├── internal/                               # Internal configuration
│   ├── lint-configs/                      # Code linting configurations
│   │   ├── eslint/                        # ESLint rules
│   │   └── prettier/                      # Prettier configuration
│   └── vite-config/                       # Vite build configuration
│       ├── base/                          # Basic configuration
│       └── plugins/                       # Plugin configuration
├── playground/                             # Development playground
├── docs/                                   # Documentation
│   ├── api/                               # API documentation
│   ├── components/                        # Component documentation
│   └── guides/                            # Usage guides
├── scripts/                                # Build scripts
│   ├── build.js                           # Build script
│   ├── dev.js                             # Development script
│   └── deploy.js                          # Deployment script
├── .github/                                # GitHub configuration
│   ├── workflows/                         # CI/CD workflows
│   └── ISSUE_TEMPLATE/                    # Issue templates
├── .vscode/                                # VS Code configuration
│   ├── extensions.json                    # Recommended extensions
│   └── settings.json                      # Workspace settings
├── LICENSE                                 # MIT License
├── package.json                            # Root package configuration
├── pnpm-workspace.yaml                    # pnpm workspace configuration
├── README.md                               # Project documentation (Chinese)
├── README_EN.md                            # Project documentation (English)
└── tsconfig.json                           # TypeScript configuration
```

---

## 🤝 Contributing Guidelines

### How to Contribute
1. **Fork the Repository**: Fork this repository to your personal account
2. **Create a Branch**: Create a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit Changes**: Commit your changes (`git commit -m 'Add amazing feature'`)
4. **Push Branch**: Push to the branch (`git push origin feature/amazing-feature`)
5. **Submit PR**: Submit a Pull Request to the main repository

### Synchronizing Upstream Code
```bash
# Add upstream repository
git remote add upstream https://github.com/original-owner/seemse-ai-admin.git

# Fetch upstream updates
git fetch upstream

# Merge upstream code
git merge upstream/main

# Push to your repository
git push origin main
```

### Contribution Standards
- **Code Style**: Follow the project's ESLint and Prettier configuration
- **Commit Messages**: Use clear commit messages, following the Conventional Commits specification
- **Documentation**: Update relevant documentation and comments
- **Testing**: Ensure code passes all tests
- **No Breaking Changes**: Avoid making destructive changes to existing functionality

## 🐛 Issue Feedback

### Bug Report Requirements
When submitting a Bug report, please include the following information:
- **Problem Description**: Clear description of the problem
- **Reproduction Steps**: Detailed steps to reproduce the issue
- **Expected Behavior**: Description of the expected correct behavior
- **Actual Behavior**: Description of the actual incorrect behavior
- **Environment Information**: Operating system, browser version, Node.js version, etc.
- **Screenshots**: If applicable, provide relevant screenshots
- **Error Logs**: Provide relevant error log information

### Feature Requests
- **Feature Description**: Detailed description of the desired feature
- **Use Case**: Explain why this feature is needed
- **Implementation Suggestions**: If possible, provide implementation suggestions
- **Priority**: Indicate the priority level

## 📄 License

This project is licensed under the [MIT License](LICENSE). You are free to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the software.

**MIT License Brief:**
- ✅ Commercial use allowed
- ✅ Modification allowed
- ✅ Distribution allowed
- ✅ Private use allowed
- ❌ Liability
- ❌ Warranty

For the full license text, please see the [LICENSE](LICENSE) file.

## 📞 Contact and References

### Project Links
- **Frontend Repository**: https://github.com/your-username/seemse-ai-admin
- **Backend Repository**: https://github.com/your-username/seemse-ai-backend
- **Official Documentation**: https://docs.seemse-ai.com
- **Online Demo**: https://demo.seemse-ai.com

### Technical Support
- **Issue Tracker**: [GitHub Issues](https://github.com/your-username/seemse-ai-admin/issues)
- **Discussions**: [GitHub Discussions](https://github.com/your-username/seemse-ai-admin/discussions)
- **Email**: support@seemse-ai.com
- **Community**: [Discord Community](https://discord.gg/seemse-ai)

### Related Projects
- **RuoYi-AI**: https://github.com/yangzongzhuan/RuoYi-AI (Upstream Project)
- **Vue 3**: https://vuejs.org/ (Frontend Framework)
- **Ant Design Vue**: https://antdv.com/ (UI Component Library)
- **Spring Boot**: https://spring.io/projects/spring-boot (Backend Framework)

---

**Make AI capability management simpler, more professional, and more secure!** 🚀