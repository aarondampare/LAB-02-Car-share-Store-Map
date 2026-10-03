# University Enrollment DDD

## 1. Problem Description

The university needs a course enrollment system where students can register for courses.

The system must ensure that:

- A student cannot register for more than 6 courses.
- Once enrollment is finalized, courses cannot be removed.

## 2. Aggregate Root

The Aggregate Root is **CourseEnrollment**.

It manages the student's enrollment and protects the business rules.

### CourseEnrollment

- Student
- Courses
- Enrollment Status

## 3. Invariants

The system has two main invariants:

1. A student cannot register for more than 6 courses.
2. Once enrollment is finalized, courses cannot be removed.

## 4. Domain Operations

### addCourse(course)

Checks whether the student has reached the maximum of 6 courses.

### removeCourse(course)

Checks whether enrollment has been finalized.

### finalizeEnrollment()

Finalizes the enrollment and emits the `CourseEnrollmentCompleted` domain event.

## 5. Domain Event

**CourseEnrollmentCompleted**

This event represents something that has already happened: the student's enrollment has been successfully completed.

## 6. Logic Flow

Student

↓

Selects courses

↓

CourseEnrollment Aggregate Root

↓

Checks business rules

↓

Allows or rejects operation

↓

Finalizes enrollment

↓

CourseEnrollmentCompleted
