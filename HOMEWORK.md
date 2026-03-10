# Lab 2: JUnit Testing - Homework Assignment

## Overview

This homework assignment is designed to reinforce the JUnit 5 testing concepts you learned in Lab 2. You'll apply nested test classes, parameterized tests, repeated tests, and various assertion techniques to test new functionality in the Online School system.

## Learning Objectives

By completing this homework, you will:
- Practice writing organized test suites using nested test classes
- Master parameterized tests with different data sources
- Implement repeated tests for reliability verification
- Apply proper test lifecycle management (@BeforeEach, @AfterEach)
- Use advanced assertions and exception testing
- Follow the Arrange-Act-Assert (AAA) pattern

## Prerequisites

- Completed Lab 2: JUnit Testing
- Understanding of JUnit 5 annotations and features
- Familiarity with the Student and Course domain models

---

## Assignment 1: Teacher Testing Suite (40 points)

### Task
Create a comprehensive test suite for a `Teacher` class with nested test organization.

### Requirements

1. **Create the Teacher class** in `src/main/java/com/bootcamp/onlineschool/model/Teacher.java`:
   - Fields: `id`, `name`, `email`, `department`, `yearsOfExperience`, `courses` (List)
   - Constructor with validation (email must contain @, yearsOfExperience >= 0)
   - Methods: `addCourse()`, `removeCourse()`, `getCourseCount()`, `isExperienced()` (>= 5 years)

2. **Create test class** `TeacherTest.java` with the following nested test classes:
   - `ConstructorTests` - Test valid/invalid teacher creation (5 tests)
   - `CourseManagementTests` - Test adding/removing courses (6 tests)
   - `ExperienceTests` - Test experience-related logic (4 tests)
   - `ValidationTests` - Test email and input validation (5 tests)

3. **Use proper annotations:**
   - @DisplayName for all test classes and methods
   - @BeforeEach for test setup
   - @Test for standard tests
   - @Nested for organization

### Grading Criteria
- Teacher class implementation: 10 points
- Test organization and structure: 10 points
- Test coverage (20 tests minimum): 15 points
- Proper use of assertions: 5 points

---

## Assignment 2: Parameterized Testing (30 points)

### Task
Write parameterized tests for the `StudentRegistry` class to test bulk operations.

### Requirements

1. **Create test class** `StudentRegistryParameterizedTest.java` with:

2. **Email Validation Tests** using `@ValueSource`:
   - Test 10 different valid email formats
   - Test 10 different invalid email formats
   - Use `@ParameterizedTest` with descriptive display names

3. **GPA Boundary Tests** using `@CsvSource`:
   - Test GPA values: 0.0, 1.5, 2.0, 2.5, 3.0, 3.5, 4.0
   - Include student ID, name, email, and GPA
   - Verify correct GPA assignment and retrieval

4. **Bulk Student Creation** using `@MethodSource`:
   - Create a method that returns Stream<Arguments> with 15 student records
   - Test adding all students and verify registry state
   - Test finding each student by ID

### Grading Criteria
- @ValueSource tests (10 email tests): 10 points
- @CsvSource tests (7 GPA tests): 10 points
- @MethodSource tests (bulk operations): 10 points

---

## Assignment 3: Course Enrollment System (30 points)

### Task
Extend the `Course` class and create comprehensive tests for enrollment scenarios.

### Requirements

1. **Add to Course class**:
   - `maxCapacity` field (default 30)
   - `waitlist` (List of Students)
   - Methods: `isFull()`, `addToWaitlist()`, `getAvailableSeats()`

2. **Create test class** `CourseEnrollmentAdvancedTest.java` with nested classes:

3. **CapacityTests** (8 tests):
   - Test enrollment up to capacity
   - Test enrollment beyond capacity
   - Test available seats calculation
   - Test isFull() method

4. **WaitlistTests** (7 tests):
   - Test adding to waitlist when full
   - Test waitlist order (FIFO)
   - Test moving from waitlist to enrolled
   - Test waitlist capacity limits

5. **RepeatedEnrollmentTests** (5 tests):
   - Use @RepeatedTest(10) to test concurrent enrollment scenarios
   - Verify state consistency after repeated operations
   - Test enrollment/drop cycles

### Grading Criteria
- Course class enhancements: 8 points
- CapacityTests implementation: 10 points
- WaitlistTests implementation: 8 points
- RepeatedTests implementation: 4 points

---

## Bonus Challenges (20 extra points)

### Challenge 1: Custom Parameterized Test (10 points)
Create a custom `@CsvFileSource` test that reads student data from a CSV file:
- Create `test-students.csv` in `src/test/resources/`
- Include 20 student records
- Write parameterized test to process all records
- Verify data integrity

### Challenge 2: Test Performance (10 points)
Create a nested test class `PerformanceTests`:
- Test registry operations with 1000 students
- Measure and assert operation time limits
- Use @RepeatedTest(5) to verify consistency
- Test search performance with large datasets

---

## Submission Guidelines

### What to Submit
1. All Java source files (Teacher.java, enhanced Course.java)
2. All test files (TeacherTest.java, StudentRegistryParameterizedTest.java, CourseEnrollmentAdvancedTest.java)
3. CSV file if attempting bonus challenge
4. Screenshot of test results showing all tests passing

### Test Execution
Your submission must pass all tests:
```bash
mvn clean test
```

Expected output:
```
[INFO] Tests run: 70, Failures: 0, Errors: 0, Skipped: 0
```

### Code Quality Requirements
- Follow Java naming conventions
- Include JavaDoc comments for all public methods
- Use meaningful variable names
- Proper indentation and formatting
- No compiler warnings

---

## Tips for Success

1. **Start with Assignment 1** - It builds foundation for others
2. **Run tests frequently** - Use `mvn test` after each test method
3. **Follow AAA pattern** - Arrange, Act, Assert in every test
4. **Use descriptive names** - @DisplayName should explain what's being tested
5. **Test edge cases** - Null values, empty lists, boundary conditions
6. **Organize logically** - Group related tests in nested classes
7. **Read error messages** - JUnit provides helpful failure information

## Common Pitfalls to Avoid

- ❌ Not using @BeforeEach for test setup
- ❌ Testing multiple things in one test method
- ❌ Forgetting to test exception scenarios
- ❌ Not using assertAll for multiple related assertions
- ❌ Hardcoding test data instead of using parameterized tests
- ❌ Ignoring test isolation (tests affecting each other)

## Resources

- JUnit 5 User Guide: https://junit.org/junit5/docs/current/user-guide/
- Lab 2 README.md - Review testing patterns
- StudentRegistryAdvancedTest.java - Reference implementation
- CourseTest.java - Nested test examples

---

## Due Date

**Submit by:** [Instructor to specify]

**Late Policy:** [Instructor to specify]

## Questions?

If you have questions about the assignment:
1. Review the Lab 2 documentation and example tests
2. Check the JUnit 5 documentation
3. Ask in the course discussion forum
4. Attend office hours

---

**Good luck! Remember: Good tests are as important as good code!** 🚀
