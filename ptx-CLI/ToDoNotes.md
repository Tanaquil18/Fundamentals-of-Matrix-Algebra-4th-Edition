[ ] General: 
  - spacing concerns?  "keep it tight?"
  - As You Read... should they be Reading Questions?
  - Consistent Capitalization in my titles
  - [x] problems with "math followed by punctuation" eating up the next space. (I think this was just my html viewer or it's been fixed.)
  - statements of examples and exercises to show, not solutions.
  - "Exercise Group" words appear now, and I'm not sure I like that
  - [x] get rid of periods after titles of subsections, other things? (feature, not a bug)

[ ] sec_existence: picture

[ ] sec_matrices: center or right-justify within a side by side?

[ ] sec_gaussian_elimination: center or right-justify within a side by side?

[ ] sec_solving_systems... can't get spacing right on \xrightarrow[\mathrm{rref}] between matrices. 

[ ] sec_matrix_multiplication... Example with Row and Column Multiplication... why no arrow over u in the last part of the question?  It's in the ptx file.  something to do with the 3 columns but only 5 problems?

[ ] sec_matrix_multiplication... (and previous sections, like sec_existence) best practices says to use \text, not font changing.  But it doesn't look right, not centered, etc.  particularly the dimensions match and output diagram in this section. Alex Jordan gave a hack that works for this section.   

[x]mathtools package... already using xrightarrow in a different section... so is it working already or not?

[ ] sec_geom_1... missing pictures, (numbers are all off because I added subsections) figure 2.3.1, 2.3.3, 2.3.5, 2.3.6, 2.3.9, 2.3.10, 2.3.12, 2.3.14, 2.3.17, 2.3.19, 2.3.23, 2.3.29, 2.3.31, and tons of pictures in the exercises.

[ ] added subsections to sec_geom_1... any unintended consequences of that?

[ ] sec_geom_1... fix/split figure 2.3.22.  Need part for the example, and part (or whole thing again) for the solution.

[ ] sec_geom_1... key insights have titles, not term (changed).  Add to index or glossary?

[ ] changed to \xrightarrow[\text{  rref  }] \quad in sec_vector_solutions and sec_solving_systems, need to change it in all previous sections.  search for qquad and replace.

[ ] sec_vector_solutions, Examples with 2 free variables, 3 free variables, and unique solution, underbrace text is not centered.  tried mathclap like in sec_matrix_multiplication, but it doesn't seem to change it.  overleaf looks even worse.  Maybe because it's part of the aligned math?  \underbrace{\vec{x_p}}_{\text{particular solution}}+ \underbrace{x_3\vec{u}+x_4\vec{v}+x_5\vec{w}}_{\text{solution to homogeneous equations } A\vec{x}=\vec{0}}

[ ] sec_solve_axb I have a sbsgroup where I've set the width to 20% and that seems to align them horizontally.  Not sure that's right, or how it will look on different size screens or print.  

[ ] sec_inverses The \xrightarrow[\text{ rref }] \quad all don't look right in this section, even though I copy-pasted from sec_solve_axb, where it looks fine.  

[ ] sec_inverse_prop has the same \xrightarrow[\text{ rref }] \quad problem as last section. 

[ ] sec_inverse_prop I couldn't get the labels on the Invertible Matrix Theorem to be alphabetical using marker, but label worked.  I didn't get a warning using CLI like I did before with xsltproc, so I just left it label.  marker worked in other cases, including once this section, so is it different because it's inside a theorem?

[x] Have gone over every section in the first two chapters making fixes!