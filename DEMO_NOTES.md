# Demo Version - Commented Features

## Features Currently Commented Out (for instructor demo):

### 1. Admin Dashboard Advanced Features
- **Agent Management Tab** - Complete agent CRUD operations
- **Customer Assignment Tab** - Assign customers to agents
- Located in: `admin-dashboard.ts` and `admin-dashboard.html`

### 2. File Upload System
- **Document Upload in Policy Applications**
  - Aadhar Card upload
  - PAN Card upload  
  - Bank Passbook upload
- Located in: `policy-apply.ts` and `policy-apply.html`

## Current Demo Features:
✅ User Authentication (Login/Register)
✅ Policy Management (CRUD) - **WITH NEW EDIT FEATURE**
✅ Policy Applications (simplified without file uploads)
✅ Claims Management
✅ Role-based Access Control (Admin/User)
✅ Responsive Bootstrap UI

## To Restore Advanced Features:
1. Uncomment imports in `admin-dashboard.ts`
2. Uncomment tabs and content in `admin-dashboard.html`
3. Uncomment file upload code in `policy-apply.ts`
4. Uncomment file upload HTML in `policy-apply.html`
5. Change `createApplication()` back to `createApplicationWithDocuments()` in policy-apply.ts

## Key Demo Points:
- **NEW**: Admin can now EDIT existing policies (just added!)
- Clean, professional UI with Bootstrap 5
- JWT Authentication working
- Database integration with Entity Framework
- RESTful API architecture
- Role-based dashboard differences