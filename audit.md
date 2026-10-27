# Audit: Struct-to-Dict Conversion in Python

| No. | README Claim                                                                                      | Verdict       | Evidence from the Code                                                                                                                                                               |
| --: | ------------------------------------------------------------------------------------------------- | ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
|   1 | The project demonstrates converting a Python dataclass object into a dictionary using `asdict()`. | **Supported** | The code imports `asdict` from `dataclasses` and uses `student_dict = asdict(student)` to convert the object into a dictionary.                                                      |
|   2 | A `Student` dataclass defines the student's name, age, and course.                                | **Supported** | The `@dataclass` decorator is applied to `Student`, which defines `name: str`, `age: int`, and `course: str`.                                                                        |
|   3 | A `Student` object is created with sample information.                                            | **Supported** | `student = Student("Rahul", 20, "AI/ML")` creates an object with sample name, age, and course values.                                                                                |
|   4 | The `asdict()` function converts the object into a dictionary.                                    | **Supported** | `student_dict = asdict(student)` converts the dataclass instance into a dictionary containing its fields and values.                                                                 |
|   5 | The resulting dictionary is printed.                                                              | **Supported** | `print(student_dict)` displays the resulting dictionary.                                                                                                                             |
|   6 | Python 3.7 or later is required.                                                                  | **Supported** | The code uses the `dataclasses` module, which was introduced in Python 3.7.                                                                                                          |
|   7 | The user should open a terminal in the folder containing `struct-to-dict.py`.                     | **Supported** | The script can be executed from a terminal when the file is accessible from the current directory or its path is specified.                                                          |
|   8 | The command `python struct-to-dict.py` runs the program.                                          | **Supported** | The code is valid Python and uses the standard-library `dataclasses` module. The command works when the file has the specified name and `python` points to a compatible interpreter. |
|   9 | The program demonstrates Python dataclasses.                                                      | **Supported** | The `@dataclass` decorator defines the `Student` class as a dataclass.                                                                                                               |
|  10 | The program demonstrates objects and attributes.                                                  | **Supported** | The `student` variable stores a `Student` instance, whose attributes are `name`, `age`, and `course`.                                                                                |
|  11 | The program demonstrates dictionaries and key-value pairs.                                        | **Supported** | `asdict(student)` produces a dictionary containing keys such as `"name"`, `"age"`, and `"course"`, with their corresponding values.                                                  |
|  12 | The program demonstrates converting a dataclass object into a dictionary.                         | **Supported** | `student_dict = asdict(student)` explicitly performs the conversion.                                                                                                                 |

## Audit Summary

* **Total claims audited:** 12
* **Supported:** 12
* **Not Supported:** 0

### Conclusion

All README claims are supported by the provided Python code. The program defines a `Student` dataclass, creates an instance, converts it into a dictionary using `asdict()`, and prints the result.

**Expected output:**

```python
{'name': 'Rahul', 'age': 20, 'course': 'AI/ML'}
```

No README changes have been made.
