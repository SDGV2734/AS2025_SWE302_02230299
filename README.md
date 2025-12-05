# SWE302 Software Testing & Quality Assurance - Practicals Repository

## Overview

This repository contains a comprehensive collection of software testing and quality assurance practicals for the **SWE302 module**. Each practical demonstrates different aspects of modern software testing, security practices, and quality assurance methodologies. The repository showcases a complete DevSecOps workflow with automation, security scanning, and performance testing.

**Student:** Sonam Dorji  
**Module:** SWE302 Software Testing & Quality Assurance  
**Repository:** AS2025_SWE302_02230299

---

## Repository Structure

This repository is organized into 8 main practicals plus supplementary practical variants (4a and 4b), each focusing on specific testing methodologies:

```
practicals/
├── practical_1/          # React Quiz Application - E2E Testing
├── practical_2/          # Go CRUD Testing - Unit Tests & Code Coverage
├── practical_3/          # Specification-Based Testing - Equivalence & Boundary Analysis
├── practical_4/          # SAST with Snyk Integration in GitHub Actions
├── practical_4a/         # SAST with SonarCloud in GitHub Actions
├── practical_4b/         # DAST with OWASP ZAP in GitHub Actions
├── practical_5/          # Integration Testing with TestContainers
├── practical_6/          # Infrastructure as Code Security with Terraform & Trivy
├── practical_7/          # Performance Testing with k6
└── practical_8/          # GUI Testing with Cypress
```

---

## Practical Descriptions & Learning Outcomes

### 📋 Practical 1: React Quiz Application - E2E Testing

**Focus:** End-to-End (E2E) Testing with Playwright for React Applications

**Description:**  
Comprehensive E2E testing implementation for a modern React Quiz application. This practical demonstrates building automated test suites for interactive user interfaces with real-time features like timers and score tracking.

**Key Components:**

- Modern React 19.0.0 with TypeScript and Tailwind CSS
- Interactive quiz with 30-second countdown timer
- Component-based architecture with custom hooks
- Playwright E2E test automation
- Docker containerization

**Technology Stack:** React, TypeScript, Vite, Tailwind CSS, Playwright, Docker

**Learning Outcomes:**

- Understand E2E testing principles and best practices
- Write automated tests for interactive UI components
- Implement timer-dependent testing scenarios
- Test responsive design across different screen sizes
- Containerize applications for consistent testing environments

**Directory:** `practical_1/`

---

### 🧪 Practical 2: Go CRUD Testing - Unit Tests & Code Coverage

**Focus:** Unit Testing and Code Coverage Analysis in Go

**Description:**  
Demonstrates fundamental unit testing practices in Go with a simple CRUD API. This practical emphasizes test-driven development and measuring code quality through coverage metrics.

**Key Components:**

- RESTful API implementation in Go
- CRUD operations for data management
- Comprehensive unit test suite
- Code coverage reporting and visualization
- HTML coverage report generation

**Technology Stack:** Go, HTTP Server, Testing Framework

**Learning Outcomes:**

- Write effective unit tests in Go
- Understand code coverage metrics
- Generate and interpret coverage reports
- Test HTTP handlers and API endpoints
- Implement best practices for testable code

**Directory:** `practical_2/`

---

### 🎯 Practical 3: Specification-Based Testing - Equivalence & Boundary Analysis

**Focus:** Specification-Based Testing Techniques

**Description:**  
In-depth coverage of specification-based testing methodologies including equivalence partitioning, boundary value analysis, and decision table testing. Uses a shipping fee calculator as a practical example.

**Key Concepts:**

- **Equivalence Partitioning:** Dividing input space into equivalence classes
- **Boundary Value Analysis:** Testing at partition boundaries (off-by-one errors)
- **Decision Table Testing:** Systematic combination of inputs and outcomes
- **Specification-First Approach:** Tests designed from requirements, not implementation

**Test Case Coverage:**

- Weight validation (negative, zero, valid ranges, overflow)
- Zone classification (domestic, international, express)
- Insurance option handling
- Edge cases and boundary conditions

**Learning Outcomes:**

- Apply specification-based testing techniques effectively
- Design test cases using equivalence partitions
- Identify and test boundary values
- Create decision tables for complex business rules
- Minimize test cases while maximizing coverage

**Directory:** `practical_3/`

---

### 🔒 Practical 4: SAST with Snyk Integration in GitHub Actions

**Focus:** Static Application Security Testing (SAST) - Snyk Integration

**Description:**  
Demonstrates DevSecOps practices by integrating Snyk security scanning into a Spring Boot 3.4.10 REST API application with GitHub Actions automation. Complete vulnerability remediation workflow.

**Security Results:**

- **Initial Vulnerabilities:** 22 security issues identified
- **Remediation Rate:** 100% (22/22 resolved)
- **Coverage:** Container images (10), Java dependencies (9), Framework (1), CI/CD (2)
- **Final Status:** Zero known vulnerabilities

**Key Features:**

- Automated Snyk scanning on code push
- Vulnerability identification and severity classification
- Systematic remediation and dependency updates
- Container image security analysis
- Compliance validation

**Technology Stack:** Spring Boot 3.4.10, Java 17, Maven, Docker, Snyk, GitHub Actions

**Learning Outcomes:**

- Integrate SAST tools into CI/CD pipelines
- Understand vulnerability severity and impact
- Remediate security issues systematically
- Implement security-first development practices
- Monitor dependencies for known vulnerabilities

**Directory:** `practical_4/`

---

### 🔍 Practical 4a: SAST with SonarCloud in GitHub Actions

**Focus:** Static Application Security Testing (SAST) - SonarCloud Integration

**Description:**  
Implements code quality analysis and security scanning using SonarCloud with GitHub Actions. Demonstrates quality gates, maintainability metrics, and comprehensive test coverage requirements.

**Quality Metrics Achieved:**

- **Security Grade:** A
- **Reliability Grade:** A
- **Code Coverage:** 93.3% (exceeds 85% target)
- **Quality Gate:** Passed
- **Maintainability:** High

**Key Components:**

- SonarCloud integration and configuration
- Quality gate enforcement
- Security hotspot detection (8 identified and managed)
- Test coverage validation
- Maintainability index assessment

**Technology Stack:** SonarCloud, GitHub Actions, Quality Gates

**Learning Outcomes:**

- Configure SonarCloud for automated code analysis
- Understand security grades and reliability metrics
- Achieve high code coverage targets
- Implement quality gates in CI/CD
- Monitor code maintainability over time

**Directory:** `practical_4a/`

---

### 🛡️ Practical 4b: DAST with OWASP ZAP in GitHub Actions

**Focus:** Dynamic Application Security Testing (DAST) - OWASP ZAP

**Description:**  
Implements runtime security analysis using OWASP ZAP for dynamic vulnerability detection. Demonstrates both baseline scanning and comprehensive security testing integrated into GitHub Actions.

**Security Analysis:**

- **Vulnerabilities Identified:** 2 critical issues
- **Remediation Status:** 100% (2/2 resolved)
- **Scan Types:** Baseline scan and full scan
- **Runtime Coverage:** Application tested while running
- **Integration:** Fully automated GitHub Actions workflow

**Key Features:**

- Baseline security scan establishment
- Full comprehensive security scan execution
- Critical vulnerability identification and remediation
- Automated scan reports with actionable insights
- Input validation and injection risk testing

**Technology Stack:** OWASP ZAP, Spring Boot, GitHub Actions, Docker

**Learning Outcomes:**

- Perform dynamic security testing at runtime
- Identify web application vulnerabilities (OWASP Top 10)
- Understand SAST vs. DAST approaches
- Implement automated security scanning in pipelines
- Remediate runtime security vulnerabilities

**Directory:** `practical_4b/`

---

### 📦 Practical 5: Integration Testing with TestContainers

**Focus:** Integration Testing - TestContainers for Database Testing

**Description:**  
Demonstrates comprehensive integration testing using TestContainers with PostgreSQL. Tests CRUD operations in a production-like isolated environment with automatic container lifecycle management.

**Test Coverage:**

- **Code Coverage:** 83% (21/25 functions)
- **Test Pass Rate:** 100% (38/38 tests)
- **Test Functions:** 16 comprehensive integration tests
- **Exercises:** 5/5 completed (100%)

**Key Features:**

- PostgreSQL container lifecycle management
- CRUD operation testing with real database
- Advanced query and filtering validation
- Transaction behavior and ACID compliance testing
- Multi-container architecture preparation
- Automatic resource cleanup

**Technology Stack:** Go, PostgreSQL, TestContainers, Docker

**Learning Outcomes:**

- Set up integration testing environments with containers
- Test database operations realistically
- Validate transaction behavior and data integrity
- Manage container lifecycle in tests
- Design maintainable integration test suites
- Achieve high code coverage metrics

**Directory:** `practical_5/`

---

### 🏗️ Practical 6: Infrastructure as Code Security with Terraform & Trivy

**Focus:** IaC Security - Terraform Configuration and Vulnerability Scanning

**Description:**  
Demonstrates secure Infrastructure as Code practices using Terraform with LocalStack AWS emulation. Includes automated vulnerability scanning with Trivy and compliance validation against industry standards.

**Security Results:**

- **Initial Vulnerabilities:** 15 security issues identified
- **Remediation:** 100% (15/15 resolved)
- **Final Status:** Zero vulnerabilities
- **Compliance:** CIS, PCI-DSS, HIPAA, NIST, SOC 2 standards

**Infrastructure Components:**

- Secure S3 bucket configuration
- Encryption and access controls
- Static website hosting (Next.js)
- AWS resource management with Terraform
- Security scanning and compliance validation

**Technology Stack:** Terraform, LocalStack, AWS, Trivy, KMS, S3

**Learning Outcomes:**

- Write secure Infrastructure as Code
- Identify and remediate IaC vulnerabilities
- Implement encryption and access controls
- Validate compliance with security standards
- Automate infrastructure security scanning
- Deploy production-ready cloud infrastructure

**Directory:** `practical_6/`

---

### ⚡ Practical 7: Performance Testing with k6

**Focus:** Performance Testing - Load and Stress Testing

**Description:**  
Comprehensive performance testing implementation for a Dog CEO API Next.js application. Covers multiple testing scenarios including smoke, load, spike, stress, and soak tests with measurable performance metrics.

**Test Scenarios Completed:**

- **Smoke Testing:** Baseline functionality validation (1 VU, 30s)
- **Average Load Testing:** Normal operating conditions (10 VU, 1m)
- **Spike Load Testing:** Sudden traffic surge handling
- **Stress Testing:** Breaking point identification (500 VU)
- **Soak Testing:** Long-duration stability verification
- **Concurrent User Testing:** Resource management validation
- **Page Load Testing:** Frontend performance metrics
- **API Endpoint Testing:** Backend performance analysis

**Performance Metrics:**

- **Response Time (avg):** 150–250ms (normal load)
- **Peak Response Time:** ~500–2000ms (under stress)
- **Error Rate (normal):** 0–0.2%
- **Error Rate (stress):** Up to 15% (at breaking point)
- **Max Concurrent Users:** 500 VUs tested

**Technology Stack:** k6, JavaScript, Next.js, Open-source load testing

**Learning Outcomes:**

- Perform comprehensive load and stress testing
- Identify system capacity and breaking points
- Measure and optimize response times
- Analyze error rates under various conditions
- Create realistic performance test scenarios
- Document performance characteristics and recommendations

**Directory:** `practical_7/`

---

### 🎨 Practical 8: GUI Testing with Cypress

**Focus:** GUI Testing - End-to-End Testing for Web Applications

**Description:**  
Implements comprehensive GUI testing using Cypress for a Next.js web application. Demonstrates UI validation, user interaction testing, API mocking, and complete user journey testing.

**Test Coverage:**

- **Total Test Scenarios:** 25+ comprehensive tests
- **Pass Rate:** 100%
- **Test Files:** 8 comprehensive test modules
- **Custom Commands:** 3 reusable functions
- **Page Objects:** Full DogBrowserPage implementation
- **API Mocking:** cy.intercept() with fixtures

**Test Categories:**
| Test File | Scenarios | Type | Pass Rate |
|-----------|-----------|------|-----------|
| Homepage Testing | 4 | UI Validation | 100% |
| Fetch Dog Tests | 5 | User Interaction | 100% |
| API Mocking | 4 | Request Interception | 100% |
| API Validation | 3 | Response Validation | 100% |
| Custom Commands | 3 | Reusable Functions | 100% |
| Fixtures | 2 | Mock Data Management | 100% |

**Key Features:**

- Page load and element visibility validation
- User interaction patterns (clicks, filtering)
- API response mocking and validation
- Custom command creation for reusability
- Page object model implementation
- Fixture-based test data management

**Technology Stack:** Cypress, TypeScript, Next.js, API Mocking

**Learning Outcomes:**

- Write effective GUI tests with Cypress
- Implement page object patterns
- Mock API responses for isolated testing
- Create custom reusable commands
- Test complete user journeys
- Validate data integrity across UI layers

**Directory:** `practical_8/`

---

## Quick Navigation

| Practical    | Focus Area          | Technology          | Key Metric               |
| ------------ | ------------------- | ------------------- | ------------------------ |
| Practical 1  | E2E Testing         | React, Playwright   | Full UI Automation       |
| Practical 2  | Unit Testing        | Go, Coverage        | 93.3% Coverage           |
| Practical 3  | Test Design         | Testing Techniques  | Equivalence Partitioning |
| Practical 4  | SAST (Snyk)         | Security, DevSecOps | Zero Vulnerabilities     |
| Practical 4a | SAST (SonarCloud)   | Code Quality        | Grade A Security         |
| Practical 4b | DAST (ZAP)          | Runtime Security    | Zero Vulnerabilities     |
| Practical 5  | Integration Testing | TestContainers      | 83% Coverage             |
| Practical 6  | IaC Security        | Terraform, Trivy    | 100% Compliance          |
| Practical 7  | Performance Testing | k6, Load Testing    | 500 VU Capacity          |
| Practical 8  | GUI Testing         | Cypress, UI Testing | 100% Pass Rate           |

---

## Walkthrough & How to Use This Repository

### Prerequisites

Before getting started, ensure you have:

- Git installed for cloning and version control
- Docker (for containerized tests and applications)
- Language-specific tools:
  - Node.js 18+ (for React, Cypress, k6)
  - Go 1.20+ (for Go CRUD testing)
  - Java 17 LTS (for Spring Boot practicals)
  - Python 3.8+ (for Terraform and general scripting)

### Getting Started

1. **Clone the Repository**

   ```bash
   git clone https://github.com/SDGV2734/AS2025_SWE302_02230299.git
   cd practicals
   ```

2. **Explore Each Practical**
   Navigate to any practical folder and read its `README.md` for specific setup and execution instructions.

### Running Each Practical

#### Practical 1: React Quiz Application

```bash
cd practical_1
npm install
npm run dev           # Start development server
npm run test:e2e      # Run Playwright tests
```

#### Practical 2: Go CRUD Testing

```bash
cd practical_2
go mod download
go test -v -cover     # Run tests with coverage
go tool cover -html=coverage.out  # Generate coverage report
```

#### Practical 3: Specification-Based Testing

```bash
cd practical_3
# Review the test cases and specifications documented in the README
# Run tests using your preferred testing framework
```

#### Practical 4: Snyk SAST Integration

```bash
cd practical_4
# View GitHub Actions workflow in .github/workflows/
# Results visible in GitHub Actions tab
# Check vulnerability reports in the README
```

#### Practical 4a: SonarCloud SAST

```bash
cd practical_4a
# GitHub Actions runs automatically on push
# View quality metrics on SonarCloud dashboard
# Check quality gate status in Actions
```

#### Practical 4b: OWASP ZAP DAST

```bash
cd practical_4b
# GitHub Actions runs DAST scanning
# View security scan reports in Actions output
# Check baseline and full scan results
```

#### Practical 5: Integration Testing with TestContainers

```bash
cd practical_5
go mod download
go test -v                    # Run all tests
go test -v -cover             # Run with coverage
docker ps                      # Verify PostgreSQL container
```

#### Practical 6: IaC Security with Terraform

```bash
cd practical_6
terraform init
terraform plan              # Preview changes
terraform apply             # Deploy infrastructure
trivy config ./             # Scan for vulnerabilities
```

#### Practical 7: Performance Testing with k6

```bash
cd practical_7
k6 run smoke-test.js           # Smoke test
k6 run average-load-test.js    # Load test
k6 run stress-test.js          # Stress test
```

#### Practical 8: GUI Testing with Cypress

```bash
cd practical_8
npm install
npm run dev           # Start Next.js app
npm run test:e2e      # Run Cypress tests
npm run test:e2e:ui   # Open Cypress UI for interactive testing
```

---

## Key DevSecOps Practices Demonstrated

This repository showcases modern DevSecOps practices across all practicals:

### 🔐 Security (Sec)

- Static Application Security Testing (SAST)
- Dynamic Application Security Testing (DAST)
- Infrastructure as Code security scanning
- Dependency vulnerability management
- Container security analysis

### 🔄 Automation (DevOps)

- GitHub Actions CI/CD pipeline
- Automated testing on code push
- Docker containerization
- Infrastructure automation with Terraform
- Continuous security monitoring

### ✅ Quality

- Unit testing and code coverage
- Integration testing with containers
- End-to-end testing automation
- Performance testing and load analysis
- GUI testing and user journey validation

### 📊 Monitoring & Reporting

- Code quality metrics (SonarCloud)
- Security vulnerability tracking
- Test coverage reporting
- Performance metrics analysis
- Compliance validation

---

## Learning Path Recommendations

### For Beginners

1. Start with **Practical 3** - Understand testing fundamentals
2. Move to **Practical 2** - Learn unit testing basics
3. Explore **Practical 1** - See E2E testing in action
4. Review **Practical 8** - Understand GUI automation

### For Intermediate Learners

1. Complete **Practical 4** and **Practical 4a** - Learn security testing
2. Work through **Practical 5** - Master integration testing
3. Study **Practical 7** - Understand performance testing

### For Advanced Learners

1. Tackle **Practical 4b** - Implement runtime security testing
2. Master **Practical 6** - Secure infrastructure automation
3. Implement **Practical 7** - Advanced performance analysis
4. Combine all practicals - Build comprehensive testing strategy

---

## Key Achievements Summary

| Metric                          | Achievement                           |
| ------------------------------- | ------------------------------------- |
| **Total Practicals**            | 10 (including 4a & 4b variants)       |
| **Total Vulnerabilities Fixed** | 100+ (across all security practicals) |
| **Code Coverage**               | 83-93.3% across multiple projects     |
| **Test Automation**             | 100+ automated test scenarios         |
| **Performance Testing**         | 8 different load profiles tested      |
| **Infrastructure Security**     | 100% compliance with 5+ standards     |
| **CI/CD Integration**           | Complete GitHub Actions automation    |

---

## Additional Resources

- **Testing Frameworks Documentation:**

  - [Playwright](https://playwright.dev/)
  - [Cypress](https://docs.cypress.io/)
  - [k6](https://k6.io/docs/)
  - [TestContainers](https://testcontainers.com/)

- **Security Tools:**

  - [Snyk](https://snyk.io/)
  - [SonarCloud](https://www.sonarsource.com/products/sonarcloud/)
  - [OWASP ZAP](https://www.zaproxy.org/)
  - [Trivy](https://github.com/aquasecurity/trivy)

- **Infrastructure & DevOps:**
  - [Terraform](https://www.terraform.io/)
  - [Docker](https://www.docker.com/)
  - [GitHub Actions](https://github.com/features/actions)

---

## Contact & Support

**Student:** Sonam Dorji  
**Email:** [Your Email]  
**GitHub:** [@SDGV2734](https://github.com/SDGV2734)

For questions or issues related to specific practicals, refer to the individual practical READMEs or create an issue in the repository.

---

## License

This repository contains practical assignments for SWE302 Software Testing & Quality Assurance course.

---

**Repository:** AS2025_SWE302_02230299
