# CECS 326 Reading Assignment: Filesystems
## 20 points

### Assignment Description
Answer the following questions from the Chapter 6 reading from your textbook. Be complete with your answers. You may work on these questions with one or two other partners, but *all* students must submit the document individually in their own repositories along with each student's name documented with the submission.


1. Is the open system call in UNIX absolutely essential? What would the consequences be of not having it?

2. A simple operating system supports only a single directory but allows it to have arbitrarily many files with arbitrarily long file names. Can something approximating a hierarchical file system be simulated? How?

3. Describe the effects of a corrupted data block for a given file for:
    a. contiguous
    b. linked
    c. indexed (or table based)

4. Consider a file whose size varies between 4 KB and 4 MB during its lifetime. Which of the three allocation schemes (contiguous, linked and table/indexed) will be most appropriate?

5. Name one advantage of hard links over symbolic links and one advantage of symbolic links over hard links. Explain your answer.

6. Consider a 4-TB disk that uses 4-KB blocks and the free-list method. How many block addresses can be stored in one block?

7. The beginning of a free-space bitmap looks like this after the disk partition is first formatted: `1000 0000 0000 0000` (the first block is used by the root directory). The system always searches for free blocks starting at the lowest-numbered block, so after writing `file A`, which uses six blocks, the bitmap looks like this: `1111 1110 0000 0000`. Show the bitmap after each of the following additional actions:
    a. `File B` is written, using five blocks
    b. `File A` is deleted
    c. `File C` is written, using eight blocks
    d. `File B` is deleted.

8. Oliver Owl's night job at the university computing center is to change the tapes used for overnight data backups. While waiting for each tape to complete, he works on writing his thesis that proves Shakespeare's plays were written by extraterrestrial visitors. His text processor runs on the system being backed up since that is the only one they have. Is there a problem with this arrangement?

9. For an external USB hard drive attached to a computer, which is more suitable: a write-through cache or a block cache? Explain.

10. Consider an application where students' records are stored in a file. The application takes a student ID as input and subsequently reads, updates, and writes the corresponding student record; this is repeated till the application quits. Would the read-ahead technique be useful here? Why or why not?

### Deliverables
Commit the answers to the questions in a readable file to your git repository by the due date and time indicated with your repository. Approved file submission formats are: .txt, .md, .pdf. .html (renderable) or anything that is web-readable on Github. Other formats will only be accepted with *explicit approval*.
