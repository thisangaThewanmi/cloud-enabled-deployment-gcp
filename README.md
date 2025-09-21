# Cloud Enabled Deployment In Action with AWS

This repository contains four projects:

- course-service (Spring Boot + MySQL)
- student-service (Spring Boot + MongoDB)
- media-service (Spring Boot + Local file storage, can be extended to S3/MinIO)
- frontend-app (React + TypeScript)

## Backend Services

### 1. course-service
- Entity: Course(id, name, duration)
- Endpoints:
  - GET /courses
  - GET /courses/{id}
  - POST /courses
  - DELETE /courses/{id}
- Default port: 8081
- Configure MySQL settings

### 2. student-service
- Document: Student(registrationNumber, fullName, address, contact, email)
- Endpoints:
  - GET /students
  - GET /students/{id}
  - POST /students
  - DELETE /students/{id}
- Default port: 8082
- Configure MongoDB settings

### 3. media-service
- Resource: files
- Endpoints:
  - POST /files (multipart/form-data: file)
  - GET /files (list)
  - GET /files/{id} (fetch)
  - DELETE /files/{id} (delete)
- Default port: 8083
- Uses local disk storage at `./data/media` by default (override with env var `MEDIA_STORAGE_DIR`).

## Frontend (frontend-app)
- React + TypeScript + MUI + Axios + Vite app with 3 sections: Courses, Students, Media
- Scripts:
  - npm run dev (Vite dev server)
  - npm run build (TypeScript build + Vite build)
  - npm run preview (Preview built app)

## License

Licensed under the MIT License.


## Vedio Link
https://drive.google.com/file/d/1vTFq_vTft6Ivsk-tqQSgtt7rIgunA2Va/view?usp=drive_link

## Details
Name : Thisanga Thewanmi Kavindya
StudentId: 2301671099
Email: thisangat2005@gmail.com


