# Projects
[Prog_lab_01_ MERT_ARSAL.ipynb](https://github.com/user-attachments/files/22927674/Prog_lab_01_.MERT_ARSAL.ipynb)
{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "provenance": []
    },
    "kernelspec": {
      "name": "python3",
      "display_name": "Python 3"
    },
    "language_info": {
      "name": "python"
    }
  },
  "cells": [
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "sLXxHU_3cXy5"
      },
      "source": [
        "# Programming Assignment: Python Basics and Boolean Logic\n",
        "\n",
        "**Course:** Introduction to Programming  \n",
        "**Target Group:** Computer Science students  \n",
        "**Time Allocation:** 90 minutes (in-class) + additional time during the week  \n",
        "**Submission Deadline:** Next class session\n",
        "\n",
        "---\n",
        "\n",
        "## 📚 Learning Objectives\n",
        "\n",
        "By completing this assignment, you will demonstrate:\n",
        "- **Knowledge:** Understanding of Python syntax, data types, and Boolean algebra\n",
        "- **Skills:** Writing clean, documented code following PEP8 standards\n",
        "- **Social Competencies:** Problem-solving and applying programming concepts to real-world scenarios\n",
        "\n",
        "---\n",
        "\n",
        "## 📝 Instructions\n",
        "\n",
        "1. Read each task carefully\n",
        "2. Write your code in the provided code cells\n",
        "3. Run your code to test it (Shift+Enter or click the Play button)\n",
        "4. Add comments to explain your code\n",
        "5. When finished, download this notebook: File → Download → Download .ipynb\n",
        "\n",
        "---"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "8jvrJjVlcXzj"
      },
      "source": [
        "# Part 1: Variables and Basic Syntax (15 points)\n",
        "\n",
        "## Task 1.1: Variable Operations (5 points)\n",
        "\n",
        "Create a Python script that:\n",
        "1. Declares three variables: `student_name` (string), `student_age` (integer), and `gpa` (float)\n",
        "2. Assigns appropriate values to each variable\n",
        "3. Prints each variable with its type using the `type()` function\n",
        "4. Changes `student_age` to a float by adding 0.5 and prints the result with its new type\n",
        "\n",
        "**Requirements:**\n",
        "- Follow snake_case naming convention\n",
        "- Include comments explaining what each section does\n",
        "- Display output in a readable format"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "wqc3wBxhcXzt",
        "outputId": "e3beeae7-5644-49e6-885a-a2bddd8561ec"
      },
      "source": [
        "# Task 1.1: Variable Operations\n",
        "# Write your code below\n",
        "\n",
        "# TODO: Declare and assign values to variables\n",
        "student_name = \"John Snow\"\n",
        "student_age = 20\n",
        "gpa = 4.0\n",
        "\n",
        "# TODO: Print each variable with its type\n",
        "print(\"Variable name: student_name, variable type:\", type(student_name),\n",
        "      \", variable value:\", student_name)\n",
        "print(\"Variable name: student_age, variable type:\", type(student_age),\n",
        "      \", variable value:\", student_age)\n",
        "print(\"Variable name: gpa, variable type:\", type(gpa),\n",
        "      \", variable value:\", gpa)\n",
        "\n",
        "# TODO: Change student_age to float and print with new type\n",
        "student_age = student_age + 0.5\n",
        "print(\"Variable name: student_age, variable type:\", type(student_age),\n",
        "      \", variable value: \", student_age)"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Variable name: student_name, variable type: <class 'str'> , variable value: John Snow\n",
            "Variable name: student_age, variable type: <class 'int'> , variable value: 20\n",
            "Variable name: gpa, variable type: <class 'float'> , variable value: 4.0\n",
            "Variable name: student_age, variable type: <class 'float'> , variable value:  20.5\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "iIxpniMMcXz9"
      },
      "source": [
        "---\n",
        "\n",
        "## Task 1.2: Long Calculations (5 points)\n",
        "\n",
        "Write a program that calculates a student's final grade using the following formula:\n",
        "\n",
        "```\n",
        "final_grade = (midterm_exam * 0.3) + (project_score * 0.25) + (homework_avg * 0.15) + (final_exam * 0.3)\n",
        "```\n",
        "\n",
        "**Requirements:**\n",
        "- The calculation should span multiple lines using the line continuation character `\\`\n",
        "- Maximum line length: 79 characters (PEP8 standard)\n",
        "- Use meaningful variable names\n",
        "- Include a docstring at the beginning explaining what the program does\n",
        "- Print the final grade with an appropriate message"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "kEg6atw-cXz-",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "6d08db7d-56a5-4b77-8208-97d7e483084f"
      },
      "source": [
        "# Task 1.2: Long Calculations\n",
        "\n",
        "\"\"\"\n",
        "TODO: Add your docstring here explaining what this program does\n",
        "\"\"\"\n",
        "\n",
        "# TODO: Declare grade component variables\n",
        "midterm_exam = 85  # Replace with actual value\n",
        "project_score = 90  # Replace with actual value\n",
        "homework_avg = 88  # Replace with actual value\n",
        "final_exam = 92  # Replace with actual value\n",
        "\n",
        "# TODO: Calculate final_grade using line continuation (\\)\n",
        "# Make sure to follow PEP8 (max 79 characters per line)\n",
        "final_grade = (midterm_exam * 0.25) + \\\n",
        "              (project_score * 0.25) + \\\n",
        "              (homework_avg * 0.20) + \\\n",
        "              (final_exam * 0.30)\n",
        "  # Replace with your calculation\n",
        "\n",
        "# TODO: Print the result with a meaningful message\n",
        "print(f\"The student's final grade is: {final_grade:.2f}\")\n"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "The student's final grade is: 88.95\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "6ooRJO7scX0E"
      },
      "source": [
        "---\n",
        "\n",
        "## Task 1.3: Code Documentation (5 points)\n",
        "\n",
        "Review the following code and improve it by:\n",
        "1. Adding appropriate comments\n",
        "2. Adding a docstring\n",
        "3. Fixing any PEP8 violations\n",
        "\n",
        "**Original Code:**\n",
        "```python\n",
        "x=10\n",
        "y=20\n",
        "z=x+y\n",
        "print(z)\n",
        "a=x*y\n",
        "print(a)\n",
        "result=z+a\n",
        "print(result)\n",
        "```"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "nrW8ow_jcX0F",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "03f05f57-6fde-4e35-8572-85bee38e4aee"
      },
      "source": [
        "# Task 1.3: Code Documentation\n",
        "# Improve the code below by adding docstring, comments, and fixing PEP8 violations\n",
        "\n",
        "# Assigning integer values to variables\n",
        "x = 10\n",
        "y = 20\n",
        "\n",
        "# Performing addition\n",
        "z = x + y\n",
        "print(\"Sum (x + y):\", z)\n",
        "\n",
        "# Performing multiplication\n",
        "a = x * y\n",
        "print(\"Product (x * y):\", a)\n",
        "\n",
        "# Calculating final result (sum + product)\n",
        "result = z + a\n",
        "print(\"Final result (z + a):\", result)"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Sum (x + y): 30\n",
            "Product (x * y): 200\n",
            "Final result (z + a): 230\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "QhgkNDm3cX0H"
      },
      "source": [
        "---\n",
        "\n",
        "# Part 2: Data Types and Type Conversion (15 points)\n",
        "\n",
        "## Task 2.1: Type Exploration (7 points)\n",
        "\n",
        "Create a program that:\n",
        "1. Creates variables of each basic type: `None`, `bool`, `int`, `float`, `str`\n",
        "2. Performs operations showing type conversion:\n",
        "   - Convert an integer to float\n",
        "   - Convert a float to integer (and explain what happens)\n",
        "   - Convert a string containing a number to integer\n",
        "   - Create a boolean from a comparison operation\n",
        "3. Document what happens to the data during each conversion\n",
        "\n",
        "**Expected Output Example:**\n",
        "```\n",
        "Original value: 10, Type: <class 'int'>\n",
        "After adding 3.5: 13.5, Type: <class 'float'>\n",
        "```"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "LiRX1oJTcX0K",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "b0be7d62-efcf-4dd6-f619-5c44433aaf96"
      },
      "source": [
        "# Task 2.1: Type Exploration\n",
        "\n",
        "# TODO: Create variables of each basic type\n",
        "none_var = None\n",
        "bool_var = True\n",
        "int_var = 10\n",
        "float_var = 3.14\n",
        "str_var = \"Hello\"\n",
        "\n",
        "# TODO: Print each variable with its type\n",
        "print(\"--- Variable Types ---\")\n",
        "print(\"none_var:\", none_var, \"| type:\", type(none_var))\n",
        "print(\"bool_var:\", bool_var, \"| type:\", type(bool_var))\n",
        "print(\"int_var:\", int_var, \"| type:\", type(int_var))\n",
        "print(\"float_var:\", float_var, \"| type:\", type(float_var))\n",
        "print(\"str_var:\", str_var, \"| type:\", type(str_var))\n",
        "\n",
        "\n",
        "print(\"\\n--- Type Conversions ---\\n\")\n",
        "\n",
        "# TODO: Convert integer to float\n",
        "int_to_float = float(int_var)\n",
        "print(\"int_to_float:\", int_to_float, \"| type:\", type(int_to_float))\n",
        "\n",
        "\n",
        "# TODO: Convert float to integer (explain what happens in a comment)\n",
        "float_to_int = int(float_var)\n",
        "print(\"float_to_int:\", float_to_int, \"| type:\", type(float_to_int))\n",
        "\n",
        "\n",
        "# TODO: Convert string containing a number to integer\n",
        "num_str = \"50\"\n",
        "str_to_int = int(num_str)\n",
        "print(\"str_to_int:\", str_to_int, \"| type:\", type(str_to_int))\n",
        "\n",
        "\n",
        "\n",
        "# TODO: Create boolean from comparison operation\n",
        "is_greater = int_var > float_var\n",
        "print(\"is_greater (int_var > float_var):\", is_greater, \"| type:\", type(is_greater))\n"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "--- Variable Types ---\n",
            "none_var: None | type: <class 'NoneType'>\n",
            "bool_var: True | type: <class 'bool'>\n",
            "int_var: 10 | type: <class 'int'>\n",
            "float_var: 3.14 | type: <class 'float'>\n",
            "str_var: Hello | type: <class 'str'>\n",
            "\n",
            "--- Type Conversions ---\n",
            "\n",
            "int_to_float: 10.0 | type: <class 'float'>\n",
            "float_to_int: 3 | type: <class 'int'>\n",
            "str_to_int: 50 | type: <class 'int'>\n",
            "is_greater (int_var > float_var): True | type: <class 'bool'>\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "KCTcN92TcX0M"
      },
      "source": [
        "---\n",
        "\n",
        "## Task 2.2: String Manipulation (8 points)\n",
        "\n",
        "Write a program that:\n",
        "1. Creates three string variables containing: first name, last name, and student ID\n",
        "2. Concatenates them into a full student record\n",
        "3. Uses the `print()` function to display:\n",
        "   - The full record\n",
        "   - The length of each string\n",
        "   - Each string in uppercase and lowercase\n",
        "4. Creates a boolean variable that checks if the student ID has exactly 6 characters"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "ZXmLpvjPcX0O",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "f75058bd-d5b2-4cb4-837c-9a8e7756a611"
      },
      "source": [
        "# Task 2.2: String Manipulation\n",
        "\n",
        "# TODO: Create three string variables\n",
        "first_name = \"Mert\"\n",
        "last_name = \"Arsal\"\n",
        "student_id = \"240815\"\n",
        "\n",
        "# TODO: Concatenate into full student record\n",
        "full_record = first_name + \" \" + last_name + \" (\" + student_id + \")\"\n",
        "\n",
        "# TODO: Display the full record\n",
        "print(\"--- Student Record ---\")\n",
        "print(full_record)\n",
        "\n",
        "\n",
        "# TODO: Display length of each string\n",
        "print(\"\\n--- String Lengths ---\")\n",
        "print(\"First name length:\", len(first_name))\n",
        "print(\"Last name length:\", len(last_name))\n",
        "print(\"Student ID length:\", len(student_id))\n",
        "\n",
        "# TODO: Display each string in uppercase and lowercase\n",
        "print(\"\\n--- Case Conversions ---\")\n",
        "print(\"First name (upper):\", first_name.upper())\n",
        "print(\"First name (lower):\", first_name.lower())\n",
        "print(\"Last name (upper):\", last_name.upper())\n",
        "print(\"Last name (lower):\", last_name.lower())\n",
        "\n",
        "\n",
        "# TODO: Check if student_id has exactly 6 characters\n",
        "print(\"\\n--- ID Check ---\")\n",
        "if len(student_id) == 6:\n",
        "    print(\"✅ Student ID has exactly 6 characters.\")\n",
        "else:\n",
        "    print(\"❌ Student ID does NOT have exactly 6 characters.\")"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "--- Student Record ---\n",
            "Mert Arsal (240815)\n",
            "\n",
            "--- String Lengths ---\n",
            "First name length: 4\n",
            "Last name length: 5\n",
            "Student ID length: 6\n",
            "\n",
            "--- Case Conversions ---\n",
            "First name (upper): MERT\n",
            "First name (lower): mert\n",
            "Last name (upper): ARSAL\n",
            "Last name (lower): arsal\n",
            "\n",
            "--- ID Check ---\n",
            "✅ Student ID has exactly 6 characters.\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "lQjXZhTMcX0P"
      },
      "source": [
        "---\n",
        "\n",
        "# Part 3: Logical Operators and Boolean Algebra (30 points)\n",
        "\n",
        "## Task 3.1: Basic Boolean Operations (10 points)\n",
        "\n",
        "Write a program that tests all logical operators and comparisons:\n",
        "\n",
        "1. Create two variables: `x = 15` and `y = 20`\n",
        "2. Test and print results of:\n",
        "   - `x == y`\n",
        "   - `x != y`\n",
        "   - `x < y`\n",
        "   - `x <= y`\n",
        "   - `x > y`\n",
        "   - `x >= y`\n",
        "   - `(x < 20) and (y > 15)`\n",
        "   - `(x < 10) or (y > 15)`\n",
        "   - `not (x == y)`\n",
        "\n",
        "3. Add comments explaining what each operation tests"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "UlXKXQkEcX0Q",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "71f4df13-86c8-49aa-f406-25d17a294b88"
      },
      "source": [
        "# Task 3.1: Basic Boolean Operations\n",
        "\n",
        "# TODO: Create variables\n",
        "x = 15\n",
        "y = 20\n",
        "\n",
        "# TODO: Test equality\n",
        "print(f\"x == y: {x == y}\")  # Checks if x and y have the same value\n",
        "\n",
        "# TODO: Complete all other comparisons with explanatory comments\n",
        "\n",
        "# TODO: Test inequality\n",
        "# Checks if x and y are different\n",
        "print(f\"x != y: {x != y}\")\n",
        "\n",
        "# TODO: Test greater than\n",
        "# Checks if x is greater than y\n",
        "print(f\"x > y: {x > y}\")\n",
        "\n",
        "# TODO: Test less than\n",
        "# Checks if x is less than y\n",
        "print(f\"x < y: {x < y}\")\n",
        "\n",
        "# TODO: Test greater than or equal to\n",
        "# Checks if x is greater than or equal to y\n",
        "print(f\"x >= y: {x >= y}\")\n",
        "\n",
        "# TODO: Test less than or equal to\n",
        "# Checks if x is less than or equal to y\n",
        "print(f\"x <= y: {x <= y}\")\n",
        "\n",
        "\n",
        "\n",
        "\n",
        "\n",
        "\n",
        "\n"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "x == y: False\n",
            "x != y: True\n",
            "x > y: False\n",
            "x < y: True\n",
            "x >= y: False\n",
            "x <= y: True\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "4w_plYVYcX0R"
      },
      "source": [
        "---\n",
        "\n",
        "## Task 3.2: University Library Access System (20 points)\n",
        "\n",
        "**Scenario:** You are developing an access control system for a university library. The system needs to determine if a student can access special research materials.\n",
        "\n",
        "**Access Rules:**\n",
        "A student can access special materials if:\n",
        "- **Condition 1:** They are a graduate student (`graduate_student = True`) AND have completed research ethics training (`ethics_training = True`)\n",
        "- **OR Condition 2:** They are working on a thesis (`thesis_student = True`) AND have professor permission (`professor_permission = True`)\n",
        "- **OR Condition 3:** They are a faculty member (`is_faculty = True`)\n",
        "\n",
        "**Additional Rule:** Access is DENIED if the student has overdue books (`has_overdue_books = True`), regardless of other conditions.\n",
        "\n",
        "### Task 3.2a: Basic Implementation (8 points)"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "tNLfK-TzcX0R",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "732e8f30-a10d-4c24-f3db-157b1a0f9720"
      },
      "source": [
        "# Task 3.2a: Basic Implementation\n",
        "\n",
        "# Test Case 1: Graduate student with ethics training, no overdue books\n",
        "graduate_student = True\n",
        "ethics_training = True\n",
        "thesis_student = False\n",
        "professor_permission = False\n",
        "is_faculty = False\n",
        "has_overdue_books = False\n",
        "\n",
        "# TODO: Write if-else statement to check access\n",
        "# Your code should print either \"ACCESS GRANTED\" or \"ACCESS DENIED\"\n",
        "if graduate_student and ethics_training and not has_overdue_books:\n",
        "    print(\"ACCESS GRANTED\")\n",
        "else:\n",
        "    print(\"ACCESS DENIED\")\n",
        "\n",
        "print(\"\\n--- Test Case 1 Result Above ---\\n\")\n",
        "\n"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "ACCESS GRANTED\n",
            "\n",
            "--- Test Case 1 Result Above ---\n",
            "\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "EIGBXcFfcX0S",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "956c722c-64a9-4bf5-a898-4db20ee5950a"
      },
      "source": [
        "# Test Case 2: Thesis student with permission, but has overdue books\n",
        "graduate_student = False\n",
        "ethics_training = False\n",
        "thesis_student = True\n",
        "professor_permission = True\n",
        "is_faculty = False\n",
        "has_overdue_books = True\n",
        "\n",
        "# TODO: Copy your if-else logic here\n",
        "\n",
        "\n",
        "\n",
        "if (\n",
        "    (graduate_student and ethics_training and not has_overdue_books)\n",
        "    or (thesis_student and professor_permission and not has_overdue_books)\n",
        "    or (is_faculty and not has_overdue_books)\n",
        "):\n",
        "    print(\"ACCESS GRANTED\")\n",
        "else:\n",
        "    print(\"ACCESS DENIED\")\n",
        "\n",
        "print(\"\\n--- Test Case 2 Result Above ---\\n\")\n"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "ACCESS DENIED\n",
            "\n",
            "--- Test Case 2 Result Above ---\n",
            "\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "LREy0vREcX0T",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "04ce1276-9d70-468f-ea70-7fe335ea3e3a"
      },
      "source": [
        "# Test Case 3: Faculty member with no overdue books\n",
        "graduate_student = False\n",
        "ethics_training = False\n",
        "thesis_student = False\n",
        "professor_permission = False\n",
        "is_faculty = True\n",
        "has_overdue_books = False\n",
        "\n",
        "# TODO: Copy your if-else logic here\n",
        "if (\n",
        "    (graduate_student and ethics_training and not has_overdue_books)\n",
        "    or (thesis_student and professor_permission and not has_overdue_books)\n",
        "    or (is_faculty and not has_overdue_books)\n",
        "):\n",
        "    print(\"ACCESS GRANTED\")\n",
        "else:\n",
        "    print(\"ACCESS DENIED\")\n",
        "\n",
        "print(\"\\n--- Test Case 3 Result Above ---\\n\")"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "ACCESS GRANTED\n",
            "\n",
            "--- Test Case 3 Result Above ---\n",
            "\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "yEn4QRF4cX0V"
      },
      "source": [
        "### Task 3.2b: Code Optimization (7 points)\n",
        "\n",
        "1. Simplify your Boolean expression using De Morgan's laws where applicable\n",
        "2. Add comments explaining your simplification process\n",
        "3. Create a more readable version by breaking complex conditions into intermediate boolean variables\n",
        "\n",
        "Example:\n",
        "```python\n",
        "# Instead of one complex condition:\n",
        "if condition1 and condition2 or condition3 and condition4:\n",
        "    # do something\n",
        "\n",
        "# Use intermediate variables:\n",
        "meets_student_requirements = condition1 and condition2\n",
        "meets_special_requirements = condition3 and condition4\n",
        "if meets_student_requirements or meets_special_requirements:\n",
        "    # do something\n",
        "```"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "qtIWH71WcX0Y",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "c4d07494-645b-47cb-d52b-285e7ee066db"
      },
      "source": [
        "# Task 3.2b: Code Optimization\n",
        "\n",
        "# Test with the same first test case\n",
        "graduate_student = True\n",
        "ethics_training = True\n",
        "thesis_student = False\n",
        "professor_permission = False\n",
        "is_faculty = False\n",
        "has_overdue_books = False\n",
        "\n",
        "# TODO: Create intermediate boolean variables for readability\n",
        "# Example: meets_graduate_requirements = ...\n",
        "meets_graduate_requirements = graduate_student and ethics_training\n",
        "meets_thesis_requirements = thesis_student and professor_permission\n",
        "meets_faculty_requirements = is_faculty\n",
        "no_overdue_books = not has_overdue_books\n",
        "\n",
        "\n",
        "\n",
        "# TODO: Write simplified if-else statement using intermediate variables\n",
        "if (meets_graduate_requirements or meets_thesis_requirements or meets_faculty_requirements) and no_overdue_books:\n",
        "    print(\"ACCESS GRANTED\")\n",
        "else:\n",
        "    print(\"ACCESS DENIED\")\n",
        "\n",
        "\n"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "ACCESS GRANTED\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "VdP_VaxYcX0a"
      },
      "source": [
        "### Task 3.2c: Testing and Documentation (5 points)\n",
        "\n",
        "Create a testing table and comprehensive docstring"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "dbL3aatWcX0a"
      },
      "source": [
        "**Testing Table** (Fill in the table below in this markdown cell):\n",
        "\n",
        "| Test # | Graduate | Ethics | Thesis | Prof Permission | Faculty | Overdue | Expected Result |\n",
        "|--------|----------|--------|--------|-----------------|---------|---------|----------------|\n",
        "| 1      | True     | True   | False  | False           | False   | False   | GRANTED        |\n",
        "| 2      | False    | False  | True   | True            | False   | True    | DENIED         |\n",
        "| 3      | False    | False  | False  | False           | True    | False   | GRANTED        |\n",
        "| 4      | TODO     | TODO   | TODO   | TODO            | TODO    | TODO    | TODO           |\n",
        "| 5      | TODO     | TODO   | TODO   | TODO            | TODO    | TODO    | TODO           |"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "NDggHWC8cX0b",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "287d70c6-5c0c-44ec-f450-69127afc7be4"
      },
      "source": [
        "# Task 3.2c: Complete System with Documentation\n",
        "\n",
        "\"\"\"\n",
        "TODO: Add comprehensive docstring explaining:\n",
        "- What this system does\n",
        "- The access rules\n",
        "- Parameters used\n",
        "- How it works\n",
        "\"\"\"\n",
        "\n",
        "def check_library_access(graduate_student, ethics_training, thesis_student,\n",
        "                         professor_permission, is_faculty, has_overdue_books):\n",
        "    \"\"\"\n",
        "    TODO: Add docstring for this function\n",
        "    \"\"\"\n",
        "    # TODO: Implement your optimized logic here\n",
        "    pass\n",
        "\n",
        "    meets_graduate_requirements = graduate_student and ethics_training\n",
        "    meets_thesis_requirements = thesis_student and professor_permission\n",
        "    meets_faculty_requirements = is_faculty\n",
        "    no_overdue_books = not has_overdue_books\n",
        "\n",
        "    if (meets_graduate_requirements or meets_thesis_requirements or meets_faculty_requirements) and no_overdue_books:\n",
        "        return \"ACCESS GRANTED\"\n",
        "    else:\n",
        "        return \"ACCESS DENIED\"\n",
        "\n",
        "# TODO: Test with all 5 test cases from your table\n",
        "test_cases = [\n",
        "    (True, True, False, False, False, False),\n",
        "    (False, False, True, True, False, True),\n",
        "    (False, False, False, False, True, False),\n",
        "    (True, False, False, False, False, False),\n",
        "    (False, True, True, False, False, False)\n",
        "]\n",
        "\n",
        "for i, case in enumerate(test_cases, 1):\n",
        "    result = check_library_access(*case)\n",
        "    print(f\"Test {i}: {result}\")\n"
      ],
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Test 1: ACCESS GRANTED\n",
            "Test 2: ACCESS DENIED\n",
            "Test 3: ACCESS GRANTED\n",
            "Test 4: ACCESS DENIED\n",
            "Test 5: ACCESS DENIED\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "1F90boK6cX0b"
      },
      "source": [
        "---\n",
        "\n",
        "# Part 4: Real-World Application (20 points)\n",
        "\n",
        "## Task 4.1: Student Scholarship Eligibility System\n",
        "\n",
        "Create a program that determines if a student qualifies for different types of scholarships.\n",
        "\n",
        "**Scholarship Types and Criteria:**\n",
        "\n",
        "**Merit Scholarship:**\n",
        "- GPA >= 3.5\n",
        "- Completed at least 30 credits\n",
        "- No academic probation\n",
        "\n",
        "**Need-Based Scholarship:**\n",
        "- Family income < 50000\n",
        "- GPA >= 2.5\n",
        "- Enrolled full-time (>= 12 credits)\n",
        "\n",
        "**Athletic Scholarship:**\n",
        "- Is a varsity athlete\n",
        "- GPA >= 2.0\n",
        "- Good standing with athletic department (no violations)\n",
        "\n",
        "**Special Achievement Scholarship:**\n",
        "- Has won a major competition OR published a research paper\n",
        "- GPA >= 3.0\n",
        "- Recommended by faculty\n",
        "\n",
        "### Implementation with PEP8 Standards (20 points)"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "Uyo3Gvn-cX0c",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "c23fc035-8ecd-4909-cce1-d0ff70f5094a"
      },
      "source": [
        "# Task 4.1: Student Scholarship Eligibility System\n",
        "\n",
        "\"\"\"\n",
        "TODO: Add module docstring explaining the scholarship system\n",
        "\"\"\"\n",
        "\n",
        "# Student Profile 1: High-achieving student\n",
        "# TODO: Set appropriate values for a student who should qualify for\n",
        "# multiple scholarships\n",
        "gpa = 3.9\n",
        "credits_completed = 120\n",
        "academic_probation = False\n",
        "family_income = 18000\n",
        "full_time_enrollment = True\n",
        "is_varsity_athlete = True\n",
        "athletic_violations = False\n",
        "won_competition = True\n",
        "published_paper = True\n",
        "faculty_recommendation = True\n",
        "\n",
        "print(\"=== Student Profile 1 ===\")\n",
        "print(f\"GPA: {gpa}, Credits: {credits_completed}\")\n",
        "print(f\"Family Income: ${family_income}\\n\")\n",
        "\n",
        "# TODO: Check Merit Scholarship eligibility\n",
        "if gpa >= 3.5 and credits_completed >= 60 and not academic_probation:\n",
        "    print(\"Eligible for: Merit Scholarship\")\n",
        "else:\n",
        "    print(\"Not eligible for: Merit Scholarship\")\n",
        "\n",
        "# TODO: Check Need-Based Scholarship eligibility\n",
        "if family_income < 25000 and full_time_enrollment and not academic_probation:\n",
        "    print(\"Eligible for: Need-Based Scholarship\")\n",
        "else:\n",
        "    print(\"Not eligible for: Need-Based Scholarship\")\n",
        "\n",
        "\n",
        "# TODO: Check Athletic Scholarship eligibility\n",
        "if is_varsity_athlete and not athletic_violations and full_time_enrollment:\n",
        "    print(\"Eligible for: Athletic Scholarship\")\n",
        "else:\n",
        "    print(\"Not eligible for: Athletic Scholarship\")\n",
        "\n",
        "# TODO: Check Special Achievement Scholarship eligibility\n",
        "if (won_competition or published_paper or faculty_recommendation) and not academic_probation:\n",
        "    print(\"Eligible for: Special Achievement Scholarship\")\n",
        "else:\n",
        "    print(\"Not eligible for: Special Achievement Scholarship\")\n",
        "\n",
        "print(\"\\n\" + \"=\"*50 + \"\\n\")"
      ],
      "execution_count": 2,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "=== Student Profile 1 ===\n",
            "GPA: 3.9, Credits: 120\n",
            "Family Income: $18000\n",
            "\n",
            "Eligible for: Merit Scholarship\n",
            "Eligible for: Need-Based Scholarship\n",
            "Eligible for: Athletic Scholarship\n",
            "Eligible for: Special Achievement Scholarship\n",
            "\n",
            "==================================================\n",
            "\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "sOdQzimqcX0d",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "b8c83b6c-8b20-4983-9c7d-98d94e1ee267"
      },
      "source": [
        "# Student Profile 2: Student qualifying for only one scholarship\n",
        "# TODO: Set values for this profile\n",
        "gpa = 2.5\n",
        "credits_completed = 40\n",
        "academic_probation = False\n",
        "family_income = 18000\n",
        "full_time_enrollment = True\n",
        "is_varsity_athlete = False\n",
        "athletic_violations = False\n",
        "won_competition = False\n",
        "published_paper = False\n",
        "faculty_recommendation = False\n",
        "\n",
        "print(\"=== Student Profile 2 ===\")\n",
        "print(f\"GPA: {gpa}, Credits: {credits_completed}\")\n",
        "print(f\"Family Income: ${family_income}\\n\")\n",
        "\n",
        "print(\"=== Student Profile 2 ===\")\n",
        "# TODO: Implement scholarship checks\n",
        "\n",
        "# ✅ Merit Scholarship\n",
        "if gpa >= 3.5 and credits_completed >= 60 and not academic_probation:\n",
        "    print(\"Eligible for: Merit Scholarship\")\n",
        "else:\n",
        "    print(\"Not eligible for: Merit Scholarship\")\n",
        "\n",
        "# ✅ Need-Based Scholarship\n",
        "if family_income < 25000 and full_time_enrollment and not academic_probation:\n",
        "    print(\"Eligible for: Need-Based Scholarship\")\n",
        "else:\n",
        "    print(\"Not eligible for: Need-Based Scholarship\")\n",
        "\n",
        "# ✅ Athletic Scholarship\n",
        "if is_varsity_athlete and not athletic_violations and full_time_enrollment:\n",
        "    print(\"Eligible for: Athletic Scholarship\")\n",
        "else:\n",
        "    print(\"Not eligible for: Athletic Scholarship\")\n",
        "\n",
        "# ✅ Special Achievement Scholarship\n",
        "if (won_competition or published_paper or faculty_recommendation) and not academic_probation:\n",
        "    print(\"Eligible for: Special Achievement Scholarship\")\n",
        "else:\n",
        "    print(\"Not eligible for: Special Achievement Scholarship\")\n",
        "\n",
        "print(\"\\n\" + \"=\"*50 + \"\\n\")"
      ],
      "execution_count": 4,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "=== Student Profile 2 ===\n",
            "GPA: 2.5, Credits: 40\n",
            "Family Income: $18000\n",
            "\n",
            "=== Student Profile 2 ===\n",
            "Not eligible for: Merit Scholarship\n",
            "Eligible for: Need-Based Scholarship\n",
            "Not eligible for: Athletic Scholarship\n",
            "Not eligible for: Special Achievement Scholarship\n",
            "\n",
            "==================================================\n",
            "\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "YQlh8yQecX0d",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "55137893-5359-4780-a6ba-148fb6c3e935"
      },
      "source": [
        "# Student Profile 3: Student qualifying for no scholarships\n",
        "# TODO: Set values for this profile\n",
        "gpa = 2.0\n",
        "credits_completed = 20\n",
        "academic_probation = True\n",
        "family_income = 60000\n",
        "full_time_enrollment = False\n",
        "is_varsity_athlete = False\n",
        "athletic_violations = True\n",
        "won_competition = False\n",
        "published_paper = False\n",
        "faculty_recommendation = False\n",
        "\n",
        "print(\"=== Student Profile 3 ===\")\n",
        "print(f\"GPA: {gpa}, Credits: {credits_completed}\")\n",
        "print(f\"Family Income: ${family_income}\\n\")\n",
        "\n",
        "\n",
        "print(\"=== Student Profile 3 ===\")\n",
        "# TODO: Implement scholarship checks\n",
        "\n",
        "# ✅ Merit Scholarship\n",
        "if gpa >= 3.5 and credits_completed >= 60 and not academic_probation:\n",
        "    print(\"Eligible for: Merit Scholarship\")\n",
        "else:\n",
        "    print(\"Not eligible for: Merit Scholarship\")\n",
        "\n",
        "# ✅ Need-Based Scholarship\n",
        "if family_income < 25000 and full_time_enrollment and not academic_probation:\n",
        "    print(\"Eligible for: Need-Based Scholarship\")\n",
        "else:\n",
        "    print(\"Not eligible for: Need-Based Scholarship\")\n",
        "\n",
        "# ✅ Athletic Scholarship\n",
        "if is_varsity_athlete and not athletic_violations and full_time_enrollment:\n",
        "    print(\"Eligible for: Athletic Scholarship\")\n",
        "else:\n",
        "    print(\"Not eligible for: Athletic Scholarship\")\n",
        "\n",
        "# ✅ Special Achievement Scholarship\n",
        "if (won_competition or published_paper or faculty_recommendation) and not academic_probation:\n",
        "    print(\"Eligible for: Special Achievement Scholarship\")\n",
        "else:\n",
        "    print(\"Not eligible for: Special Achievement Scholarship\")\n",
        "\n",
        "print(\"\\n\" + \"-\"*50 + \"\\n\")\n",
        "\n",
        "print(\"\\n\" + \"=\"*50 + \"\\n\")"
      ],
      "execution_count": 5,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "=== Student Profile 3 ===\n",
            "GPA: 2.0, Credits: 20\n",
            "Family Income: $60000\n",
            "\n",
            "=== Student Profile 3 ===\n",
            "Not eligible for: Merit Scholarship\n",
            "Not eligible for: Need-Based Scholarship\n",
            "Not eligible for: Athletic Scholarship\n",
            "Not eligible for: Special Achievement Scholarship\n",
            "\n",
            "--------------------------------------------------\n",
            "\n",
            "\n",
            "==================================================\n",
            "\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "PKvNyR7ncX0e"
      },
      "source": [
        "### Bonus Challenge (+5 points)\n",
        "\n",
        "Add a feature that calculates the total scholarship amount:\n",
        "- Merit Scholarship: $5,000\n",
        "- Need-Based Scholarship: $3,000\n",
        "- Athletic Scholarship: $4,000\n",
        "- Special Achievement Scholarship: $2,500"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "93syQ9SycX0e",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "7850376b-8066-4cee-e3b0-138f88d70398"
      },
      "source": [
        "# Bonus: Calculate total scholarship amount\n",
        "\n",
        "def calculate_total_scholarship(merit, need_based, athletic, special):\n",
        "\n",
        "\n",
        "    MERIT_AMOUNT = 5000\n",
        "    NEED_BASED_AMOUNT = 3000\n",
        "    ATHLETIC_AMOUNT = 4000\n",
        "    SPECIAL_AMOUNT = 2500\n",
        "\n",
        "    total = 0\n",
        "\n",
        "    if merit:\n",
        "        total += MERIT_AMOUNT\n",
        "    if need_based:\n",
        "        total += NEED_BASED_AMOUNT\n",
        "    if athletic:\n",
        "        total += ATHLETIC_AMOUNT\n",
        "    if special:\n",
        "        total += SPECIAL_AMOUNT\n",
        "\n",
        "    return total\n",
        "\n",
        "# TODO: Test with your student profiles\n",
        "total1 = calculate_total_scholarship(True, True, False, True)\n",
        "print(f\"Student 1 Total Scholarship: ${total1}\")\n",
        "\n",
        "# Student Profile 2: Only Need-Based\n",
        "total2 = calculate_total_scholarship(False, True, False, False)\n",
        "print(f\"Student 2 Total Scholarship: ${total2}\")\n",
        "\n",
        "# Student Profile 3: No scholarships\n",
        "total3 = calculate_total_scholarship(False, False, False, False)\n",
        "print(f\"Student 3 Total Scholarship: ${total3}\")\n",
        "\n",
        "\n"
      ],
      "execution_count": 10,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Student 1 Total Scholarship: $10500\n",
            "Student 2 Total Scholarship: $3000\n",
            "Student 3 Total Scholarship: $0\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "FjVVc_IscX0f"
      },
      "source": [
        "---\n",
        "\n",
        "# Reflection Section\n",
        "\n",
        "## Your Learning Reflection (10 points)\n",
        "\n",
        "Write at least 200 words reflecting on:\n",
        "1. What you learned from this assignment\n",
        "2. Which task was most challenging and why\n",
        "3. How you can apply Boolean logic in real-world programming\n",
        "4. What concepts you want to explore further\n",
        "\n",
        "**Write your reflection in the markdown cell below:**"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "FRNVUt6xcX0g"
      },
      "source": [
        "### My Reflection\n",
        "\n",
        "TODO: Write your reflection here (minimum 200 words)\n",
        "\n",
        "[Your reflection goes here...]"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "hqZc7qxMcX0h"
      },
      "source": [
        "---\n",
        "\n",
        "# Submission Checklist\n",
        "\n",
        "Before submitting, make sure you have:\n",
        "\n",
        "- [ ] Completed all tasks in Parts 1-4\n",
        "- [ ] Added appropriate comments to your code\n",
        "- [ ] Added docstrings where required\n",
        "- [ ] Followed PEP8 standards (line length, naming conventions, spacing)\n",
        "- [ ] Tested all your code (all cells run without errors)\n",
        "- [ ] Filled in the testing table in Task 3.2c\n",
        "- [ ] Written your reflection (minimum 200 words)\n",
        "- [ ] (Optional) Completed the bonus challenge\n",
        "\n",
        "## How to Submit\n",
        "\n",
        "1. Make sure all cells have been run and show output\n",
        "2. Go to: **File → Download → Download .ipynb**\n",
        "3. Submit the downloaded file to your course management system\n",
        "4. File name should be: `lastname_firstname_programming_Ex_01.ipynb`\n",
        "\n",
        "---\n",
        "\n",
        "## Grading Rubric\n",
        "\n",
        "| Criterion | Points | Description |\n",
        "|-----------|--------|-------------|\n",
        "| **Correctness** | 40 | Programs work as specified |\n",
        "| **Code Quality** | 20 | PEP8 compliance, readability, structure |\n",
        "| **Documentation** | 15 | Comments, docstrings, clear explanations |\n",
        "| **Testing** | 15 | Adequate test cases, documented results |\n",
        "| **Reflection** | 10 | Understanding demonstrated in written reflection |\n",
        "| **Bonus** | +5 | Additional features or exceptional quality |\n",
        "| **TOTAL** | **100** | (+5 bonus) |\n",
        "\n",
        "---\n",
        "\n",
        "## Additional Resources\n",
        "\n",
        "- [Python Documentation](https://docs.python.org/3/)\n",
        "- [PEP8 Style Guide](https://pep8.org/)\n",
        "- [Google Colab Tips](https://colab.research.google.com/notebooks/basic_features_overview.ipynb)\n",
        "\n",
        "**Good luck, and happy coding!** 🐍"
      ]
    }
  ]
}
