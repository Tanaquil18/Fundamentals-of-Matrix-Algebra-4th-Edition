-[ ] General: 
  - spacing concerns?  "keep it tight?"
  - As You Read... should they be Reading Questions?
  - Consistent Capitalization in my titles
  - [x] problems with "math followed by punctuation" eating up the next space. (I think this was just my html viewer or it's been fixed.)
  - [x] statements of examples and exercises to show, not solutions (unknowled in publication file)
  - "Exercise Group" words appear now, and I'm not sure I like that
  - [x] get rid of periods after titles of subsections, other things? (feature, not a bug)

-[x] have no generated pictures anywhere yet

-[ ] sec_matrices: center or right-justify within a side by side?

-[ ] sec_gaussian_elimination: center or right-justify within a side by side?

-[x] sec_solving_systems... can't get spacing right on \xrightarrow[\mathrm{rref}] between matrices. 

-[x] sec_matrix_multiplication... Example with Row and Column Multiplication... why no arrow over u in the last part of the question?  It's in the ptx file.  something to do with the 3 columns but only 5 problems? (must have been my html viewer... looks fine now!)

-[x] sec_matrix_multiplication... (and previous sections, like sec_existence) best practices says to use \text, not font changing.  But it doesn't look right, not centered, etc.  particularly the dimensions match and output diagram in this section. (\mathclap seems to have solved it for this particular problem. based on output seem in mathjax, I kind of want to try removing the mathclap now, but not enough to risk creating a problem where there currently isn't one.)  

-[x]mathtools package... already using xrightarrow in a different section... so is it working already or not?

-[ ] added subsections to sec_geom_1... any unintended consequences of that?

-[x] sec_geom_1... fix/split figure 2.3.22.  Need part for the example, and part (or whole thing again) for the solution.

-[x] sec_geom_1... some pictures are gigantic.  fix individually, or as a group?  exercises, knowls, etc? (fixed in lin_trans, geom_1, existence, and vector_solutions... still need to fix in later sections)

-[ ] pictures in later sections, need xml:id's with sensible names, and width="60%"

-[ ] sec_geom_1... key insights have titles, not term (changed).  Add to index or glossary?

-[x] changed to \xrightarrow[\text{  rref  }] \quad in sec_vector_solutions and sec_solving_systems, need to change it in all previous sections.  search for qquad and replace. (removed the \quad and added a macro instead.  couldn't get brackets to work for going under the arrow, so I went with braces for going above the arrow. )

-[ ] does the above mean I don't need to load mathtools anymore?

-[ ] sec_vector_solutions, Examples with 2 free variables, 3 free variables, and unique solution, underbrace text is not centered.  tried mathclap like in sec_matrix_multiplication, but it doesn't seem to change it.  overleaf looks even worse.  Maybe because it's part of the aligned math?  \underbrace{\vec{x_p}}_{\text{particular solution}}+ \underbrace{x_3\vec{u}+x_4\vec{v}+x_5\vec{w}}_{\text{solution to homogeneous equations } A\vec{x}=\vec{0}}

-[ ] sec_determinant_1 similar to above, have underbraces with text not centered.  also part of aligned math.  mathjax website looked better... maybe just a cocalc problem?

-[ ] sec_solve_axb I have a sbsgroup where I've set the width to 20% and that seems to align them horizontally.  Not sure that's right, or how it will look on different size screens or print.  

-[x] sec_inverses The \xrightarrow[\text{ rref }] \quad all don't look right in this section, even though I copy-pasted from sec_solve_axb, where it looks fine.  

-[x] Use a macro \rrefarrow in main.ptx and change it once.  Then change every section to use \rrefarrow.  See Rob's email.  

-[x] sec_inverse_prop has the same \xrightarrow[\text{ rref }] \quad problem as last section. 

-[ ] sec_inverse_prop and sec_existence I added sage cells but don't know what to do about <output>, how to format it, so I didn't include any. 

-[x] sec_inverse_prop I couldn't get the labels on the Invertible Matrix Theorem to be alphabetical using marker, but label worked.  I didn't get a warning using CLI like I did before with xsltproc, so I just left it as label.  marker worked in other instances, including one other time this section, so is it different because it's inside a theorem? (now it works... not sure what changed)
  
-[ ] sec_determinant_properties Invertible Matrix Theorem omits the middle and just has first and last equivalence... might want to change that.
  
-[ ] sec_determinant_properties Key Idea xml:id="idea_3by3shortcut" not sure I like the spacing and how that looks.

-[x] Have gone over every section in the first three chapters making fixes!
  
-[x] Starting statements of definitions, theorems, examples, etc, on a new line instead of right after the title?  Relatedly, placement of the idx markers? (checked sample article... followed its conventions)

-[ ] Have I been checking and fixing the chapter.ptx files or just the section files? I think just the section files. Do first three chapter files.

-[x] Just fixed chapter_eigen.ptx and sec_eigen.ptx  

-[ ]  Codespaces, every exercises division gets an xml-id.  Go back and add to every section before sec_eigen.ptx.
  
-[ ] Not PreTeXt related, but sec_transpose calls non-square matrices triangular... change this or add a note that some authors don't do this?
