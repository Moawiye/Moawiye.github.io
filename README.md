# Module-6-Python-programming-1
In this module, we will take a look at lists.  A list is ordered, changeable and there are many built-in methods in Python to work with lists. 
{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "anaconda-cloud": {},
    "kernelspec": {
      "display_name": "Python 3",
      "language": "python",
      "name": "python3"
    },
    "language_info": {
      "codemirror_mode": {
        "name": "ipython",
        "version": 3
      },
      "file_extension": ".py",
      "mimetype": "text/x-python",
      "name": "python",
      "nbconvert_exporter": "python",
      "pygments_lexer": "ipython3",
      "version": "3.5.4"
    },
    "colab": {
      "name": "Moawiye Moawiye ModuleSixLessonOneActivity.ipynb",
      "provenance": [],
      "include_colab_link": true
    }
  },
  "cells": [
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "view-in-github",
        "colab_type": "text"
      },
      "source": [
        "<a href=\"https://colab.research.google.com/github/Moawiye/Module-6-lesson-1/blob/main/Moawiye_Moawiye_ModuleSixLessonOneActivity.ipynb\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "ZFkhIlXF48UF"
      },
      "source": [
        "# Moawiye Moawiye\n",
        "# 10/20/2021\n",
        "# The goal of this activity was to introduce us to how string sequences work. We worked on string indexes and worked on individual string characters\n",
        "#  It was hard combining input with ifs and string sequences "
      ],
      "execution_count": 17,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "J561rEqL1MA3"
      },
      "source": [
        "# Module Six Lesson One Practice Activity\n",
        "## String Sequences\n",
        "- **Accessing string characters with index**\n",
        "- Accessing substrings with index slicing\n",
        "- Iterating through characters of a string\n",
        "- More string methods\n",
        "\n",
        "----- \n",
        "\n",
        "### Student will be able to\n",
        "- **Work with string characters by index**\n",
        "- Slice strings into substrings\n",
        "- Iterate through string characters\n",
        "- Use string methods"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "collapsed": true,
        "id": "YeF1sR0B1MA5"
      },
      "source": [
        "## Concept: Accessing a Single String Character\n",
        "[![view video](https://iajupyterprodblobs.blob.core.windows.net/imagecontainer/common/play_video.png)]( http://edxinteractivepage.blob.core.windows.net/edxpages/f7cff1a7-5601-48a1-95a6-fd1fdfabd20e.html?details=[{\"src\":\"http://jupyternootbookwams.streaming.mediaservices.windows.net/a8044252-4f2f-4960-b37b-70da8fe4769a/Unit2_Section1.1a-String_Index_Address.ism/manifest\",\"type\":\"application/vnd.ms-sstr+xml\"}],[{\"src\":\"http://jupyternootbookwams.streaming.mediaservices.windows.net/a8044252-4f2f-4960-b37b-70da8fe4769a/Unit2_Section1.1a-String_Index_Address.vtt\",\"srclang\":\"en\",\"kind\":\"subtitles\",\"label\":\"english\"}])\n",
        "### Addressing a string index\n",
        "Strings are sequences of characters.  Another common sequence type used in this course is a **list**.  Sequences index items counting from 0 for the first item.\n",
        "\n",
        "![string with index for each letter](https://iajupyterprodblobs.blob.core.windows.net/imagecontainer/string_indexes.PNG)  \n",
        "\n",
        "```python\n",
        "# assign string to student_name\n",
        "student_name = \"Alton\"\n",
        "# first character is at index 0\n",
        "student_name[0]\n",
        "```  \n"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "DQLQTDR81MA6"
      },
      "source": [
        "### Examples"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "collapsed": true,
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 0
        },
        "id": "2KmHKoUV1MA7",
        "outputId": "64f92cf2-496a-4d14-f50d-5b9b85709bc9"
      },
      "source": [
        "# [ ] review and run example - note the first element is always index = 0\n",
        "student_name = \"Alton\"\n",
        "print(student_name[0], \"<-- first character at index 0\")\n",
        "print(student_name[1])\n",
        "print(student_name[2])\n",
        "print(student_name[3])\n",
        "print(student_name[4])"
      ],
      "execution_count": 1,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "A <-- first character at index 0\n",
            "l\n",
            "t\n",
            "o\n",
            "n\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 0
        },
        "id": "uu9W3Tf_1MA8",
        "outputId": "5b603a6b-c567-4b0c-9c34-7f864cdff605"
      },
      "source": [
        "# [ ] review and run example\n",
        "student_name = \"Jin\"\n",
        "if student_name[0].lower() == \"a\":\n",
        "    print('Winner! Name starts with A:', student_name)\n",
        "elif student_name[0].lower() == \"j\":\n",
        "    print('Winner! Name starts with J:', student_name)\n",
        "else:\n",
        "    print('Not a match, try again tomorrow:', student_name)"
      ],
      "execution_count": 2,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Winner! Name starts with J: Jin\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 0
        },
        "id": "DxsLUdc61MA8",
        "outputId": "b4f226ff-dcbb-4851-bb0e-e20e65df2e80"
      },
      "source": [
        "# [ ] review and run ERROR example\n",
        "# cannot index out of range\n",
        "student_name = \"Tobias\"\n",
        "print(student_name[5])"
      ],
      "execution_count": 4,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "s\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "collapsed": true,
        "id": "UImzBq421MA8"
      },
      "source": [
        "## Task 1: Work with individual string characters  \n",
        "\n",
        "|                                                                 |\n",
        "|-----------------------------------------------------------------|\n",
        "| **Remember:** The first character in a string is at **index 0**.|\n",
        "|                                                                 |\n"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 0
        },
        "id": "p7tamlqK1MA9",
        "outputId": "2fc24ae8-2089-4b0c-800c-0e61482d8f85"
      },
      "source": [
        "# [ ] assign a string 5 or more letters long to the variable: street_name\n",
        "# [ ] print the 1st, 3rd and 5th characters\n",
        "street_name = \"Capstreet\"\n",
        "print(street_name[0])\n",
        "print(street_name[2])\n",
        "print(street_name[4])\n",
        "\n"
      ],
      "execution_count": 7,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "C\n",
            "p\n",
            "t\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 0
        },
        "id": "Sp7_z-YK1MA-",
        "outputId": "8ded7b30-507a-4197-f351-e6f7949ced69"
      },
      "source": [
        "# [ ] Create an input variable: team_name - ask that second letter = \"i\", \"o\", or \"u\"\n",
        "# [ ] Test if team_name 2nd character = \"i\", \"o\", or \"u\" and print a message\n",
        "# note: use if, elif and else\n",
        "team_name = input('Second should = \"i\", \"o\", or \"u\"')\n",
        "\n",
        "if team_name.isalpha():\n",
        "  if team_name[1] == \"i\" :\n",
        "    print('Second letter is \"i\"')\n",
        "  elif team_name[1] == \"o\" :\n",
        "    print('Second letter is \"o\"')\n",
        "  elif team_name[1] == \"u\" :\n",
        "    print('Second letter is \"u\"')\n",
        "  else:\n",
        "    ('Put a team that has \"i\", \"o\", or \"u\" as its second letter')\n",
        "else:\n",
        "  pass\n",
        "\n",
        "\n"
      ],
      "execution_count": 8,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Second should = \"i\", \"o\", or \"u\"dude\n",
            "Second letter is \"u\"\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "bh63j_d_1MA-"
      },
      "source": [
        "## Concept: Using a Negative Index \n",
        "[![view video](https://iajupyterprodblobs.blob.core.windows.net/imagecontainer/common/play_video.png)](http://edxinteractivepage.blob.core.windows.net/edxpages/f7cff1a7-5601-48a1-95a6-fd1fdfabd20e.html?details=[{\"src\":\"http://jupyternootbookwams.streaming.mediaservices.windows.net/28da3b48-538d-4412-ae7b-ce95e9892ce9/Unit2_Section1.1b-Using_a_Negative_Index.ism/manifest\",\"type\":\"application/vnd.ms-sstr+xml\"}],[{\"src\":\"http://jupyternootbookwams.streaming.mediaservices.windows.net/28da3b48-538d-4412-ae7b-ce95e9892ce9/Unit2_Section1.1b-Using_a_Negative_Index.vtt\",\"srclang\":\"en\",\"kind\":\"subtitles\",\"label\":\"english\"}])\n",
        "### Access the end of a string using -1\n",
        "Strings assign an **index** number address to each string character\n",
        "\n",
        "- First character in a string is index 0\n",
        "- Last character in a string is index **-1**\n",
        "\n",
        "![negative string index counts from the end](https://iajupyterprodblobs.blob.core.windows.net/imagecontainer/string_neg_index.PNG)\n",
        "\n",
        "To access the last character in a string:\n",
        "```python\n",
        "student_name[-1]\n",
        "```\n"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "0vAK75iw1MA_"
      },
      "source": [
        "### Examples\n",
        "\n"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "X_a9HQGr1MA_"
      },
      "source": [
        "#### access the last character with the -1 index\n",
        "negative index counts back from the last character in a string  "
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 0
        },
        "id": "BP5mc7KU1MA_",
        "outputId": "4fc09c32-6878-4bfe-c2fd-89d4e1151698"
      },
      "source": [
        "# [ ] review and run example\n",
        "student_name = \"Joana\"\n",
        "\n",
        "# get last letter\n",
        "end_letter = student_name[-1]\n",
        "print(student_name,\"ends with\", \"'\" + end_letter + \"'\")"
      ],
      "execution_count": 9,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Joana ends with 'a'\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 0
        },
        "id": "bJsHo14q1MBA",
        "outputId": "2097e8ac-2f18-4d67-cf73-b30b0a7f3361"
      },
      "source": [
        "# [ ] review and run example\n",
        "# get second to last letter\n",
        "second_last_letter = student_name[-2]\n",
        "print(student_name,\"has 2nd to last letter of\", \"'\" + second_last_letter + \"'\")"
      ],
      "execution_count": 10,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Joana has 2nd to last letter of 'n'\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 0
        },
        "id": "cohEgg3F1MBA",
        "outputId": "81e49ed9-1597-4673-c32a-3f399bbfc52c"
      },
      "source": [
        "# [ ] review and run example\n",
        "# you can get to the same letter with index counting + or -\n",
        "print(\"for\", student_name)\n",
        "print(\"index 3 =\", \"'\" + student_name[3] + \"'\")\n",
        "print(\"index -2 =\",\"'\" + student_name[-2] + \"'\")"
      ],
      "execution_count": 11,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "for Joana\n",
            "index 3 = 'n'\n",
            "index -2 = 'n'\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "collapsed": true,
        "id": "3-UDUiNi1MBA"
      },
      "source": [
        "## Task 2\n"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 0
        },
        "id": "k1lUYWpz1MBB",
        "outputId": "24878301-2651-40cf-8c39-87fcb550895e"
      },
      "source": [
        "# [ ] assign a string 5 or more letters long to the variable: street_name\n",
        "# [ ] print the last 3 characters of street_name\n",
        "street_name = \"jonny boy\"\n",
        "print(street_name[3:4:])\n"
      ],
      "execution_count": 12,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "n\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 0
        },
        "id": "A5H4F_Qy1MBB",
        "outputId": "833e1de9-4f94-4f8b-b643-11ec22a67b49"
      },
      "source": [
        "# [ ] create and assign string variable: first_name\n",
        "first_name = \"Jimmy\"\n",
        "# [ ] print the first and last letters of name\n",
        "print(first_name[0], first_name[-1])\n"
      ],
      "execution_count": 16,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "J y\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "collapsed": true,
        "id": "blMnxZXZ1MBB"
      },
      "source": [
        "## Task 3: Fix the errors"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 0
        },
        "id": "FtN0isoB1MBC",
        "outputId": "20f3b6c0-8ddc-4720-d3f5-e9999fb39a31"
      },
      "source": [
        "# [ ] Review, Run, Fix the error using string index\n",
        "shoe = \"tennis\"\n",
        "# print the last letter\n",
        "print(shoe[-1])\n",
        "\n"
      ],
      "execution_count": 15,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "s\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "LcMt03g11MBC"
      },
      "source": [
        "[Terms of use](http://go.microsoft.com/fwlink/?LinkID=206977)   [Privacy &amp; cookies](https://go.microsoft.com/fwlink/?LinkId=521839)   © 2017 Microsoft"
      ]
    }
  ]
}
