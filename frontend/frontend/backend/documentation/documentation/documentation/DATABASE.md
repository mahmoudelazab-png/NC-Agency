# NC Agency OS - Database Architecture


## 1. Users Table

Stores all system users.

Fields:

- id
- name
- email
- password
- role
- phone
- status
- created_at


Roles:

- Admin
- Account Manager
- Media Buyer
- Designer
- Content Creator
- Finance


---

## 2. Clients Table

Stores agency clients.

Fields:

- id
- company_name
- contact_person
- phone
- email
- industry
- service_package
- status
- created_at


---

## 3. Leads Table

Stores potential clients.

Fields:

- id
- name
- phone
- source
- interested_service
- status
- assigned_to
- created_at


---

## 4. Projects Table

Stores client projects.

Fields:

- id
- client_id
- project_name
- description
- start_date
- end_date
- status
- budget


---

## 5. Tasks Table

Stores team tasks.

Fields:

- id
- project_id
- assigned_user
- title
- description
- priority
- status
- deadline


---

## 6. Content Calendar Table

Stores social media content.

Fields:

- id
- client_id
- platform
- content_type
- caption
- design_file
- publish_date
- status


---

## 7. Campaigns Table

Stores advertising campaigns.

Fields:

- id
- client_id
- platform
- campaign_name
- budget
- start_date
- end_date
- results


---

## 8. Finance Table

Stores financial transactions.

Fields:

- id
- client_id
- type
- amount
- payment_status
- date


---

## 9. Notifications Table

Stores system notifications.

Fields:

- id
- user_id
- message
- status
- created_at
