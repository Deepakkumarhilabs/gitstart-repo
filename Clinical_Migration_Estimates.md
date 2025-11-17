# Clinical Migration Effort Estimation

## Executive Summary

**Total Effort:** 480 hours  
**Duration:** 60 working days (8 hours/day)  
**Timeline:** 3 months (20 working days/month)

---

## Detailed Breakdown

### 1. Login Module
- **Effort:** 4 hours
- **Type:** UI Implementation
- **Scope:** Complete user interface for login functionality

---

### 2. SideNav Module
- **Effort:** 8 hours
- **Type:** UI Implementation
- **Scope:** Complete navigation sidebar implementation

---

### 3. Dashboard Module
**Total Effort:** 38 hours

#### 3.1 Global Filters Setup (12 hours)
- **Frontend:** 6 hours - Module-wise filter configuration
- **Backend:** 6 hours
  - Factory setup methods implementation
  - JPA-based filter delivery (replacing hardcoded filters)
  - Config-driven filter management for easier future additions

#### 3.2 Data Grid Full Setup (16 hours)
- **Frontend:** 8 hours - Grid UI implementation
- **Backend:** 8 hours - Column configuration in RDS

#### 3.3 Score Cards (10 hours)
- **Frontend:** 5 hours - Chart implementation
- **Backend:** 5 hours - Filter query modifications

---

### 4. Load Tracker Module
**Total Effort:** 22 hours

#### 4.1 Filters (6 hours)
- **Backend:** Query optimization and implementation for all filters

#### 4.2 Data Grid (16 hours)
- UI implementation
- Action handlers
- Backend column configuration
- Expanded data views
- Polling functionality

---

### 5. ID-Based Loader Tracker Module
**Total Effort:** 226 hours

#### 5.1 Tabs (2 hours)
- Straightforward tab implementation

#### 5.2 Load Tracker Sub-Module (30 hours)
- **Stepper Component:** 10 hours - Build all stepper cards
- **Data Grid:** 20 hours
  - Backend column configuration
  - UI implementation

#### 5.3 File Tracker (14 hours)
- **Mini Sidebar:** 4 hours
- **Stepper + Data Grid:** 10 hours

#### 5.4 Mapping (20 hours)
- **Basic Data Grid:** 8 hours (UI + Backend)
- **Popup Data Grid:** 12 hours
  - Action implementations
  - Backend configuration

#### 5.5 Datasets (48 hours)
- **Tabs + Filters:** 14 hours - Tab structure and per-tab filter setup
- **Query Builder:** 10 hours
- **Tab Data Grids:** 24 hours - Multiple grids across different tabs

#### 5.6 Reports (96 hours)
- **Filters:** 16 hours (UI + Backend)
- **Score Cards:** 8 hours
  - UI implementation
  - Backend API modifications for filter integration
- **Data Grids:** 24 hours (UI + Backend)
- **Popup Components:** 24 hours
  - Query Builder integration
  - Dropdown rule implementation

#### 5.7 Config (36 hours)
- **Tabs + Data Grids:** 18 hours
  - 2 tabs with UI implementation
  - Backend column configuration
- **View Page Data Grids:** 18 hours
  - New page creation
  - Data grid implementation
  - Backend column setup

#### 5.8 Related Files (4 hours)
- Standard data grid implementation

---

### 6. Global Config Module
**Total Effort:** 182 hours

#### 6.1 ICM Data Grid (52 hours)
- **Data Grid:** 12 hours (UI + Backend)
- **Actions:** 8 hours
- **Action Popups:** 20 hours - Multiple popup data grids
- **Validation Rules:** 12 hours - Business logic and validation checks

#### 6.2 UCM Data Grid (52 hours)
- **Data Grid:** 12 hours (UI + Backend)
- **Actions:** 8 hours
- **Action Popups:** 20 hours - Multiple popup data grids
- **Validation Rules:** 12 hours - Business logic and validation checks

#### 6.3 Data Quality (42 hours)
- **Multi-Step Forms:** Complex forms with multiple steps
- **Popups:** Various popup implementations
- **Data Grids & Forms:** Integrated grid and form components
- **Validations:** Comprehensive validation logic

#### 6.4 Data Sources (36 hours)
- **Data Grid:** 12 hours (UI + Backend)
- **Business Rules:** 12 hours - Validation and business logic
- **Grid Features:** 12 hours
  - Filter implementation
  - Reset functionality
  - Column-level filters

---

## Summary by Module

| Module | Hours | % of Total |
|--------|-------|------------|
| Login | 4 | 0.8% |
| SideNav | 8 | 1.7% |
| Dashboard | 38 | 7.9% |
| Load Tracker | 22 | 4.6% |
| ID-Based Loader Tracker | 226 | 47.1% |
| Global Config | 182 | 37.9% |
| **TOTAL** | **480** | **100%** |

---

## Key Effort Areas

### High Complexity Components (Require More Effort):
1. **ID-Based Loader Tracker** (226 hours / 47.1%) - Most significant effort
   - Reports sub-module: 96 hours
   - Datasets sub-module: 48 hours
   - Config sub-module: 36 hours

2. **Global Config** (182 hours / 37.9%) - Second largest effort
   - ICM & UCM Data Grids: 104 hours combined
   - Data Quality: 42 hours
   - Data Sources: 36 hours

### Technology Stack:
- **Frontend:** React/Angular UI components, data grids, charts
- **Backend:** JPA queries, REST APIs, column configurations, business logic
- **Database:** RDS configuration and query optimization

### Risk Considerations:
- Multi-step form validations may require additional testing time
- Query Builder component complexity may vary based on requirements
- Integration between modules should be tested thoroughly
