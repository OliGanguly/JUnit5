# JUnit5
# unit I have to test
## Student Repo
+ selectExistsBtEmail(String):Boolean
## Student Service
   + private StudenrRepo studentRepo
   + public getAllStudents(Student):List<Student>
   + public deleteStudent(Long):void
   + public addStudent(Long):void
## Collection
   + private StudentService studentService;
  + public getAllStudents(Student):List<Student>
   + public deleteStudent(Long):void
   + public addStudent(Long):void
## steps
First Go to Your StudetRepository presss Shift + ctrl + t to create a StudentRepoTest Class

@Test = to denine it is a test method
```bash
@Autowired
private StudentRep studentRepo;
+ Implement given + when + then

@Test
    void itShouldCheckStudentExistsByEmail() {
        //given
        String email ="oli28@gamil.com";
        Student student = new Student("Oli","oli28@gmail.com",Gender.FEMALE);
        studentRepositoryUnderTest.save(student);
        //when
        Boolean expected = studentRepositoryUnderTest.selectExistsEmail(email);
        //then
        assertThat(expected).isTrue();
    }
```



