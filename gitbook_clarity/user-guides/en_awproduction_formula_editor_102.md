---
description: "EN AWProduction Formula Editor 1.02"
---



# EN AWProduction Formula Editor 1.02

Formula Editor              R




                             English




                 A+W Production
                 Introduction                                                                                Introduction




                                        Introduction
                                        In this part of the documentation you can find editorial notices.


                                        Revision Overview
                                        Part
                                        Version / Date

                                        1.00 / 11-2004             Original Version.

                                        1.01 / 07-2013             Adapted to CI 2013 layout.

                                        1.02 /01.2017              Product and company names adjusted.



                                        Editorial
                                        The editorial contains the following themes:
                                        •   Notes on this document
                                        •   Copyrights
                                        •   Trademarks
                                        •   Contact

                                        Notes on this document
                                        This document is intended only for end users of A+W Production.
                                        The documentation and software described are licenses that must be used or
                                        copied only in accordance with the conditions of our license agreement. The
                                        contents of the documentation are only informative and is subject to changes
                                        without prior notice. The text and illustrations were compiled with the utmost
                                        care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be
                                        held liable for errors or inaccuracies, unless they can be attributed to wilful or
                                        grossly negligent action.
                                        The descriptions in this document are based on the full installation of A+W
                                        Production.

                                        Copyrights
                                        © 2017, A+W Software GmbH, any right, also the right of reprint, the produc-
                                        tion of copies and of the translation, is reserved. The documentation must be
                                        copied, completely or in part, saved, or transferred only in accordance with our
                                        license agreement. Transmission of the documentation is not allowed, neither
                                        electronically, nor mechanically, nor by recording or in any other way, without
                                        A+W Software GmbH prior approval in writing.
1.02 / 01-2017




                                        Trademarks
                                        Any designation of hardware and software being mentioned in the documen-
                                        tation can also be registered trademarks or other commercial rights of third


                 A+W Production Formula Editor                                                                        R-3
                 Introduction                                                                      Introduction




                                parties being protected by law. Rights of third parties being protected by law
                                are to be observed insofar.

                                Contact
                                A+W Software GmbH

                                Am Pfahlgraben

                                D-35415 Pohlheim

                                   +49 6404 2051 0

                                   +49 6404 2051 877

                                aw.zentrale@a-w.com

                                http://www.a-w.com
1.02 / 01-2017




                 R-4                                                         A+W Production Formula Editor
                 Introduction                                                                                                                          Contents




                                        Contents
                                         Revision Overview ............................................................................................... R-3
                                         Editorial ............................................................................................................... R-3
                                        Contents ................................................................................................................. R-5

                                        Functional Principle                                                                                                R-7
                                        Formula Editor ........................................................................................................ R-9
                                          Objective of the Formula Editor ........................................................................... R-9
                                          Elements of the Formula Editor: Level I .............................................................. R-9
                                             Formula .......................................................................................................... R-10
                                             Comparison .................................................................................................... R-11
                                             Condition ........................................................................................................ R-11
                                                Linking of Elementary Conditions ............................................................... R-13
                                             Quantity .......................................................................................................... R-14
                                             Allocation ....................................................................................................... R-15
                                          Elements of the Formula Editor: Level II ........................................................... R-15
                                             Formula .......................................................................................................... R-15
                                             Comparison .................................................................................................... R-16
                                             Condition ........................................................................................................ R-16
                                             Quantity .......................................................................................................... R-17
                                             Allocation ....................................................................................................... R-18
                                          Elements of the Formula Editor: Level III .......................................................... R-18
                                             Quantity .......................................................................................................... R-18
                                        Notation Formula.dll .............................................................................................. R-20
                                          Syntax ............................................................................................................... R-20
                                             ASSIGNMENT ............................................................................................... R-20
                                             FORMULA ..................................................................................................... R-20
                                             CONDITIONS ................................................................................................ R-20
                                             CONDITION (comparison) ............................................................................. R-20
                                             SET ................................................................................................................ R-21
                                          Function ............................................................................................................. R-21
                                             ASSIGNMENT ............................................................................................... R-21
                                             FORMULA ..................................................................................................... R-22
                                             CONDITIONS ................................................................................................ R-22
                                             CONDITION ................................................................................................... R-22
                                             SET ................................................................................................................ R-23
                                          Check Results ................................................................................................... R-23
                                        List of Dialogs ....................................................................................................... R-25

                                        Operation                                                                                                        R-27
                                        Conditions for Racks ............................................................................................. R-29
                                        Conditions for Organization Groups ..................................................................... R-31
                                        Group Formation Mode ......................................................................................... R-34
                                        Conditions for Production Sections ....................................................................... R-36
                                        More Examples ..................................................................................................... R-39
1.02 / 01-2017




                 A+W Production Formula Editor                                                                                                                R-5
                 Contents                                                                                                               Introduction




                            Software Reference                                                                                                 R-43
                            Formula Editor ...................................................................................................... R-45
                              Select Conditions .............................................................................................. R-46
                              Conditions - Editor ............................................................................................. R-48
                              Condition ........................................................................................................... R-51
                              Condition Name ................................................................................................. R-53
                              Info .................................................................................................................... R-54
                                Invert .............................................................................................................. R-54
                                Given Quantity ............................................................................................... R-55
                              Enter Value (Numeric) ....................................................................................... R-55
                              Select Quantity .................................................................................................. R-57
                              Quantity Editor ................................................................................................... R-59
                              Quantity Name .................................................................................................. R-61
                              Info .................................................................................................................... R-63
                              Select Formulas ................................................................................................ R-64
                              Formula Editor ................................................................................................... R-66
                              Select Allocation ................................................................................................ R-69
                              Allocation Editor ................................................................................................ R-69

                            Partindex                                                                                                          R-73
                            Index Formula Editor ............................................................................................ R-75
1.02 / 01-2017




                 R-6                                                                                 A+W Production Formula Editor
Formula Editor                   R

                 Functional Principle




                 A+W Production
                 Functional Principle                                                                    Formula Editor




                                        Formula Editor
                                        The formula editor is available in A+W Production in the sections:
                                        •   Organization
                                        •   Machinery Allocation
                                        •   Labels, Sketches, Bender Text
                                        The formula editor has different levels. The more complex the formula, the
                                        higher the level.
                                        The documentation on the formula editor was therefore split into:
                                        •   Elements of the Formula Editor: Level I
                                        •   Elements of the Formula Editor: Level II
                                        •   Elements of the Formula Editor: Level III


                                        Objective of the Formula Editor
                                        With regards to Organization, the formula editor is used to define conditions to
                                        allocate product properties to the appropriate racks.
                                        In connection with machinery allocation, the formula editor is used to localize
                                        machinery depending on the processing, and the product properties.
                                        Regarding labels, the formula editor helps to define conditions to select the
                                        necessary label layout with regards to the product properties.


                                        Elements of the Formula Editor: Level I
                                        The formula editor consists of the elements:
                                        •   “Formula” on page R-10
                                        •   “Comparison” on page R-11
                                        •   “Condition” on page R-11
                                        •   “Quantity” on page R-14
                                        •   “Allocation” on page R-15
1.02 / 01-2017




                 A+W Production Formula Editor                                                                      R-9
                 Formula Editor                                                              Functional Principle




                                  Formula
                                  In the simplest case, a formula consists of a term which can contain the valid
                                  object properties, constants, other formulas, and some operators. Possible op-
                                  erators are the basic arithmetical operations +, -, * and / plus brackets. Also,
                                  there are the String operators:
                                  @LEFT : Syntax STRING @LEFT ANZAHL = STRING
                                  @RIGHT : Syntax STRING @RIGHT ANZAHL = STRING
                                  @MID : Syntax STRING @MID INDEX = STRING ; the index is 0-based
                                  All these operators can be mixed at random.
                                  The formula affects just one element.




                                       Formula input field


                                    This part will not be
                                          used


                                  Fig. R-1     Formula Editor


                                  Examples:
                                  $TEILETYP
                                  $MENGE * ($DICKE+1000)
                                  ($BEARB1TEXT @MID $TEILETYP) @RIGHT ($DICKE/1000)
1.02 / 01-2017




                 R-10                                                           A+W Production Formula Editor
                 Functional Principle                                                                       Formula Editor




                                        Comparison
                                        A comparison consists of 1-2 formulas, and a so-called comparison rule.
                                        Please not that you can use just one formula only if the comparison rule Only
                                        formula 1 is used. In this case, the comparison is fulfilled if the result of formula
                                        1 is one digit bigger than zero, or a non-empty string. Otherwise, the compar-
                                        ison is fulfilled if the term FORMEL 1 VORSCHRIFT FORMEL 2 is true.
                                        For formula 2, no formula needs to be defined for simple constants. In this
                                        case, activate radio button Value and enter the required constant.




                                        Fig. R-2      Comparison


                                        Examples
                                        Formula Element type = value 1
                                        Formula IG Only formula 1
                                        Formula triple width < Formula height
                                        Formula thickness = value 3 mm


                                        Condition




                                        Fig. R-3      Condition with And Connection


                                        A condition must be fulfilled so that the allocation can be made as defined by
                                        the formula(s). It is the top element within the formula structure and, in its sim-
1.02 / 01-2017




                                        plest type, consists of a number of comparisons. The grouping of comparisons
                                        defines how the results of the comparisons must be linked to each other. Com-
                                        parisons set next to another are linked by AND while comparisons set above



                 A+W Production Formula Editor                                                                         R-11
                 Formula Editor                                                                      Functional Principle




                                  one another are linked by OR. A condition is fulfilled if it is possible to find a
                                  horizontal path from left to right which only includes fulfilled comparisons.

                                  Examples:


                                    Simplest Type

                                        Condition         "Ist ESG"


                                                      "Part Type TGH"            "Only Formula 1"

                                         Formula                        Comparison


                                                                        Possible Operations:
                                                          "$T_TGH"      Only Formula, equal,
                                         Property
                                                                        unequal, smaller, smaller
                                                                        or equal, greater, greater
                                   Elementary Condition                 or equal



                                  Fig. R-4      Schematic Display of a Condition


                                  The condition is toughened glass is fulfilled if the formula element type tough-
                                  ened glass with the property of database field E_TG from Pool_Elements con-
                                  tains the value One (based on the operation only formula).




                                                                          A
                                                                          B



                                                                          C



                                  A Formula
                                  B Comparison
                                  C Elementary Condition
                                  Fig. R-5      Conditions - Author
1.02 / 01-2017




                 R-12                                                                   A+W Production Formula Editor
                 Functional Principle                                                                                Formula Editor




                                        Examples:

                                        Linking of Elementary Conditions



                                           Condition            Free Shape with Processing



                                             Formula          Comparison       Value            Formula     Comparison

                                            Shape Number           =             99            Processing    Only Formula 1



                                             Property                                           Property

                                            Shape_No                                           Processing



                                             Formula           Comparison      Value

                                                                    =            98


                                             Property

                                            Shape_No




                                         OR - Linking
                                                                                              AND - Linking

                                        Fig. R-6           Schematic Display of the Linking of Elementary Conditions




                                        Fig. R-7           Linking of Elementary Conditions
1.02 / 01-2017




                 A+W Production Formula Editor                                                                                R-13
                 Formula Editor                                                                                             Functional Principle




                                  Quantity


                                                Will not be used



                                  Fig. R-8       Quantities - Creator


                                  A quantity consists of the rule of how to form the final quantity from the start
                                  element (BOM). The following rules can be combined at random.
                                   Software Reference, “Quantity Editor” on page R-59
                                  An element can represent a processing step.


                                                                                                                         Implicit Proc.
                                                                                                                           Insulating
                                                                                                                          No Release
                                                                                                IG
                                                                                              Release
                                                                                               Part 0




                                                                                         Implicit Proc.
                                                                                          Connecting
                                                                Cast Resin                No Release                      Heat Prot.
                                                                  Release                                                No Release
                                                               Part 01000000                                            Part 02000000



                                    Condition: Is TGH
                                                                Implicit Proc.                         Implicit Proc.
                                                                 Toughening                             Toughening
                                                                 No Release                             No Release

                                                   TGH                               TGH
                                                  Release                          Release
                                               Part 1010000                      Part 1020000



                                                                Explicit Proc.       Explicit Proc.                Explicit Proc.
                                                                  Arrissing          Silk Screening                  Arrissing
                                                                 No Release              Release                    No Release



                                                    Float                             Float
                                                No Release                        No Release
                                               Part 01010100                     Part 01020100

                                  Fig. R-9       Schematic Display of the Quantity


                                  For instance, the condition is toughened glass and quantity Parent results in
                                  all final and interim products produced from one or more toughened glass el-
                                  ements.
1.02 / 01-2017




                 R-14                                                                                 A+W Production Formula Editor
                 Functional Principle                                                                        Formula Editor




                                        Allocation
                                        The simplest type is the allocation of an object property to a formula. The result
                                        of the formula is allocated to the object property.

                                        Example:
                                            EXTRA THICKNESS = formula 2mm
                                            STACK WIDTH = Height


                                        Elements of the Formula Editor: Level II
                                        The formula editor consists of the elements:
                                        •   “Formula” on page R-15
                                        •   “Comparison” on page R-16
                                        •   “Condition” on page R-16
                                        •   “Quantity” on page R-17
                                        •   “Allocation” on page R-18


                                        Formula
                                        The formula now contains a quantity plus instructions. Without the quantity, the
                                        formula directly affects the object to be checked. When a quantity is defined,
                                        the object to be checked is converted into a quantity, the object being the start
                                        object of the quantity. The formula will be applied to each object of the final
                                        quantity; the results will be linked according to instructions. If the final quantity
                                        contains no objects, a long value -1 is returned.

                                        Examples:
                                            $THICKNESS ; quantity: all basic elements; TOTAL total thickness
                                            1 ; quantity: all processings; TOTAL  number of processings
                                        Valid operations are total, average, And link, Or link, minimum and maximum.




                                        Fig. R-10     Formula
1.02 / 01-2017




                 A+W Production Formula Editor                                                                         R-15
                 Formula Editor                                                                    Functional Principle




                                  Comparison
                                  Normally, a comparison consists of 1-2 formulas and the instruction. Alterna-
                                  tively, a comparison can be expressed by a condition (activate radio button
                                  Conditions). In this case, the comparison is fulfilled if the allocated condition is
                                  fulfilled. This type of linking conditions is used whenever two or more condi-
                                  tions are applied to different quantities.




                                  Fig. R-11     Comparison


                                  Condition
                                  A condition can be inverted, i.e. it is fulfilled if the result of the comparisons is
                                  not fulfilled, and vice versa. This way, you can easily create from an existing
                                  condition the inverted one. The inverted condition contains just one compari-
                                  son which will be allocated the original condition. Moreover, the characteristic
                                  invert will be selected for the inverted condition. The status line shows INV in
                                  front of the condition name.
                                  The comparisons are usually analyzed for the object to be checked. If you
                                  want to check however whether one of the sub-elements of an object has a
                                  certain element type/processing type, you can allocate a quantity to the con-
                                  dition. In this case, the object is changed into a quantity, the object being the
                                  start object of the quantity. The condition will be analyzed for all elements of
                                  the final quantity. You only need to define when the condition is fulfilled. If it is
                                  sufficient that part of the final quantity fulfils the condition, select operation
                                  One. If the condition is only fulfilled if all elements of the final quantity fulfil the
                                  condition, select operation All. If the final quantity contains no objects, the con-
                                  dition is not fulfilled.

                                  Examples:
                                     Formula Element type = value 125 ; quantity All sub-elements ; One
                                     with processing type =125
                                     Formula E_IG Only formula 1, quantity Main element; One (or All)
                                     The main element is IG
1.02 / 01-2017




                 R-16                                                               A+W Production Formula Editor
                 Functional Principle                                                                      Formula Editor




                                                                                  with quantity




                                        Fig. R-12    Condition


                                        Quantity
                                        The quantity definition contains a condition. All objects which does not fulfil the
                                        condition, will be removed from the final quantity.

                                        Example:
                                           ; Anychild ; condition processing;
                                           -> The final quantity contains only the processings below the start element.
                                        If a condition is used, the two instructions Up and Addup can be used. These
                                        must not be combined with other instructions.
                                        Using Up means that the final quantity consists of one element only. Starting
                                        from the start element, all main elements of the start element will be checked
                                        whether they fulfil the condition. The final quantity contains the last element
                                        fulfilling the condition. Should one element fail to fulfil the condition, the up-
                                        wards iteration will be aborted
                                        Addup means that the final quantity can consist of more than one element.
                                        Like with Up, there is an upward iteration from the start element which will be
                                        stopped should one element fail to fulfil the condition. The final quantity, how-
                                        ever, contains all elements fulfilling the condition.

                                        Examples:
                                           ; Up; condition no processing
                                           ; Addup ; condition not ordered
1.02 / 01-2017




                 A+W Production Formula Editor                                                                       R-17
                 Formula Editor                                                               Functional Principle




                                  Allocation
                                  The allocation can include a quantity. In this case, the result of the formula of
                                  the property will be allocated to all objects of the final quantity.

                                  Example:
                                     EXTRA THICKNESS = Formula 2mm ; quantity All cut elements


                                  Elements of the Formula Editor: Level III

                                  Quantity
                                  Quantity definition will always be loaded with a start quantity. In simple cases,
                                  the start quantity consists of just one element, namely the start element. Dialog
                                  Quantity Editor allows to logically group several elements next to each other
                                  or below each other, like in the Conditions Editor. The elements in the Quantity
                                  Editor are different. The vertically grouped quantities form the combined quan-
                                  tity while the horizontally grouped quantities form the intersection.
                                  Please note that there is a second window for the edition of quantities. You can
                                  switch between the first and second window via button [+/-]. The start quantity
                                  is found by removing from the quantity of the first(+) window all objects of the
                                  quantity of the second(-) window.

                                  Examples:
                                  {quantity main element or Self; Anychild + Self ; ; }
                                     1st window (Plus): Quantity main element or self
                                     2nd window (Minus): empty
                                     Anychild and Self are tagged
1.02 / 01-2017




                 R-18                                                            A+W Production Formula Editor
                 Functional Principle                                                                     Formula Editor




                                        This produces a main element, and all sub-elements of the main element. If
                                        there is no main element, the final quantity includes the start element and all
                                        its sub-elements.




                                        Fig. R-13    Quantities - Creator


                                        The result is the final quantity with all elements sharing the main element of
                                        the start element.
                                        If the iteration for Up or Addup shall not start with the element itself, but with
                                        the main element, first form the start quantity from the start element, using
                                        quantity main element {;Parent;;}, and use this with the required quantity, and
                                        the instruction Up or Addup.
                                        This quantity can be allocated a formula. In this case, the formula will be ana-
                                        lyzed for all elements of the start quantity; the results will be saved. From the
                                        final quantity, all elements will be removed the start quantity of which does not
                                        contain the result of the formula.

                                        Example:
                                           ; All; ; Formula Element type
                                           Produces all elements of the BOM which are of the same type as the start
                                           element.
1.02 / 01-2017




                 A+W Production Formula Editor                                                                      R-19
                 Notation Formula.dll                                                          Functional Principle




                                        Notation Formula.dll
                                        Syntax

                                        ASSIGNMENT
                                         Input: Object, UserSet
                                            PROPERTY = FORMULA ; SET [/USERSET]


                                        FORMULA
                                         Input: Object, UserSet
                                            [ formulaelements ; SET ; OP [/USERSET] ]


                                            OP ∈ {total, average,And,Or,Minimum,Maximum}
                                            formulaelements = property , FORMULA ; + - * / ( ) 0..9 @LEFT
                                            @RIGHT @MID


                                        CONDITIONS
                                         Input: Object, UserSet
                                            ´ conditionelements ; SET ; OP [/N] [/USERSET] `
                                            OP ∈ {NULL,One,All}
                                            conditionelements =
                                            CONDITION(S)
                                            or
                                            (conditionelements OP conditionelements)    OP ∈ {And,Or}


                                        CONDITION (comparison)
                                         Input: Object, UserSet
                                            ´ FORMULA [OP FORMULA] ; ; `
                                            OP ∈ {=,!=,>,>=,<,<=}
1.02 / 01-2017




                 R-20                                                           A+W Production Formula Editor
                 Functional Principle                                                                 Notation Formula.dll




                                        SET
                                           Input; Set, UserSet
                                                 { (setelements)[-(setelements)] ; OP ; CONDITIONS ; FORMULA [/US-
                                                 ERSET] }
                                                 Note: Element ‚-(setelements)' is used only if it is not ‚empty'.
                                                 OP ∈ {All,Master,Parent,Self;Child,Anychild,Bottom,Up,Addup}
                                                 setelements =      'empty'
                                                 or
                                                 SET
                                                 or
                                                 (setelements OP setelements) OP ∈ {∩, ∪}


                                        Function

                                        ASSIGNMENT
                                        The UserSet is transferred to FORMULA and SET.
                                           •     without Set, without UserSet
                                                 The FORMULA will be analyzed for this object. The result of the FOR-
                                                 MULA is allocated to the object PROPERTY.
                                           •     With Set
                                                 SET is used to create a quantity from the given object. For every ele-
                                                 ment of this quantity, the FORMULA will be analyzed; the result will be
                                                 allocated to the PROPERTY of the corresponding object.
                                           •     With UserSet
                                                 For every object of the UserSet, the FORMULA will be analyzed; the re-
                                                 sult will be allocated to the PROPERTY of the corresponding object.
                                           •     With Set, with UserSet
                                                 Invalid, impossible.
1.02 / 01-2017




                 A+W Production Formula Editor                                                                       R-21
                 Notation Formula.dll                                                                Functional Principle




                                        FORMULA
                                        The UserSet is transferred to the SET and to all FORMULAs in formula ele-
                                        ments.
                                        •   without Set, without UserSet
                                            All formulaelements for the given object will be analyzed; the complete
                                            term will be calculated. The result is returned as MultiValue.
                                        •   With Set
                                            SET is used to create a quantity from the given object. All formulaelements
                                            for every element of this quantity will be analyzed; the complete term will
                                            be calculated. The results will be analyzed as per Operation; the total result
                                            will be returned as MultiValue.
                                        •   With UserSet
                                            All formulaelements for every element of the UserSet will be analyzed; the
                                            complete term will be calculated. The results will be analyzed as per Oper-
                                            ation; the total result will be returned as MultiValue.
                                        •   With Set, with UserSet
                                            invalid, impossible


                                        CONDITIONS
                                        The UserSet is transferred to SET and to all CONDITION(S)s in the conditio-
                                        nelements.
                                        •   without Set, without UserSet
                                            All conditionelements for the given object will be analyzed; the total result
                                            will be calculated and returned as BOOLEAN.
                                        •   With Set, (with Operation != ZERO)
                                            SET is used to create a quantity from the given object. All formulaelements
                                            for every element of this quantity will be analyzed; the complete BOOLEAN
                                            term will be calculated. If the Operation = ONE, CONDITIONS will return
                                            TRUE if for at least one element the complete BOOLEAN term is fulfilled,
                                            i.e. TRUE. If however the Operation = ALL, CONDITIONS will return TRUE
                                            if the complete BOOLEAN term is fulfilled, i.e. TRUE for all elements. Oth-
                                            erwise, FALSE will be returned.
                                        •   With UserSet
                                            All formulaelements for every element of the UserSet will be analyzed; the
                                            complete BOOLEAN term will be calculated. If the Operation = ONE, CON-
                                            DITIONS will return TRUE if for at least one element the complete BOOL-
                                            EAN term is fulfilled, i.e. TRUE. If however the Operation = ALL,
                                            CONDITIONS will return TRUE if the complete BOOLEAN term is fulfilled,
                                            i.e. TRUE for all elements. Otherwise, FALSE will be returned.
                                        •   With Set, with UserSet
                                            invalid, impossible


                                        CONDITION
                                        The UserSet is transferred to every FORMULA.
1.02 / 01-2017




                                            •   Any
                                                Both FORMULAS, if existing, will be ana lysed for the given object.



                 R-22                                                                  A+W Production Formula Editor
                 Functional Principle                                                                   Notation Formula.dll




                                        If there is only one FORMULA, TRUE will be returned if the result of FORMU-
                                        LA is not ZERO (numeric result), or if it is no empty string for string results.
                                        Otherwise, FALSE will be returned. If both FORMULAs do exist, the results will
                                        be compared acc. to the Operation. If the comparison is fulfilled, TRUE will be
                                        returned; otherwise, FALSE.


                                        SET
                                        All SETs, CONDITIONS and FORMULA included in setelements will be trans-
                                        ferred to the UserSet.
                                        •   without FORMULA, without UserSet
                                            All setelements for the given Set will be calculated; the preliminary quantity
                                            A will be determined. For every object of this quantity A, quantity BA will be
                                            determined as per Operation, to be added to quantity B. From quantity B,
                                            all objects will be removed which do not fulfil the CONDITIONS. As a result,
                                            quantity B is returned as RelatedSet.
                                        •   with FORMULA, without UserSet
                                            Initially like A, but quantity B will not be returned. The FORMULA will be an-
                                            alyzed for every object from the given Set. The results will be saved in an
                                            array. Next, the FORMULA is analyzed for every object in quantity B. If the
                                            array includes the result of the FORMULA for an object from quantity B, the
                                            corresponding object will be added to quantity C. As a result, quantity C is
                                            returned as RelatedSet.
                                        •   without FORMULA, with UserSet
                                            Like A, but instead of the given Sets, the UserSet will be used to form quan-
                                            tity A.
                                        •   with FORMULA, with UserSet
                                            Like B, but instead of the given Sets, the UserSet will be used to form quan-
                                            tity A. Still, the given Set will be used to form the array.

                                        Example:
                                        For lite A and a certain number of lites, you want to determine the total number
                                        of all lites belonging to the same route as lite A:
                                            [$MENGE ; { ; ; ; [$TOUR] /USERSET } ; SUM }
                                        Lite X shall be kept at the rack only if it is laminated glass, and if the total of all
                                        lites includes at least 150 laminated lites:
                                            ´ (´[T_VSG;;]=[1;;];;` AND ´[$MENGE;{;;´´[T_VSG;;]==[1;;]`;;`;/USER-
                                            SET};SUM]`>=[150;;]`) ; ; `


                                        Check Results
                                        To check the results of the formulas, you can view the corresponding log file.
                                        To activate the result check for Detailed Scheduling, the following setting must
                                        be made in A+W Production :
1.02 / 01-2017




                                        Master Data > Parameters > Module Detailed Scheduling > Specials > View
                                        Formula > Enter value 1




                 A+W Production Formula Editor                                                                           R-23
                 Notation Formula.dll                                                              Functional Principle




                                           Performance
                                           Viewing the calculations will impair the performance!




                                        Fig. R-14    Log file


                                        The log file for the result check is found in
                                           \<AlcimRootDir>\Log\(Name of log file of Detailed Scheduling).LOG
1.02 / 01-2017




                 R-24                                                                   A+W Production Formula Editor
                 Functional Principle                                                                          List of Dialogs




                                        List of Dialogs
                                        This list shows all dialogs you need to use the formula editor properly. The ref-
                                        erences lead to chapter Software Reference in the master data section. You
                                        will find detailed information on the dialogs, fields and buttons.

                                        Base Data Menu

                                        Menu Entry                      Dialog/Function

                                        The formula editor cannot        “Select Conditions” on page R-46
                                        be reached by means of a         “Conditions - Editor” on page R-48
                                        menu entry.                      “Condition” on page R-51
                                        The individual dialogs will
                                                                         “Condition Name” on page R-53
                                        tell you how to access it.
                                                                         “Info” on page R-63
                                                                         “Select Formulas” on page R-64
                                                                         “Formula Editor” on page R-66
                                                                         “Select Allocation” on page R-69
                                                                         “Allocation Editor” on page R-69

                                        Tab. R-1      List of Dialogs
1.02 / 01-2017




                 A+W Production Formula Editor                                                                          R-25
                 List of Dialogs              Functional Principle
1.02 / 01-2017




                 R-26              A+W Production Formula Editor
Formula Editor                R

                        Operation




                 A+W Production
                 Operation                                                                        Conditions for Racks




                                        Conditions for Racks
                                        Explains how to define, change, or delete conditions for racks in section Orga-
                                        nization.


                                         This is how you define a condition for a rack, filtering all lites with an
                                          edge length over 1,20 m
                                        1 Open the Organization Dialog via
                                           Master Data > Detailed Scheduling> Organization
                                        2 Open tab Production Sequence.
                                        3 Tag the rack for which you want to define a condition.
                                        4 Press button [New Condition]. The dialog Select Conditions --1-- appears.
                                        5 Press button [New Condition …]. This opens the dialog Conditions Editor.
                                        6 In menu Conditions, open Names. This leads to dialog Condition Name
                                          Field New Name shows New Condition by default. Give the condition a
                                          characteristic name. Example: Large Lite. Close the dialog via button [OK].
                                        7 In menu Conditions, open Info. This opens dialog Info. Enter a clear de-
                                          scription of this condition. Example: This condition is true if one edge of a
                                          lite is longer than 1,20 m. Close the dialog via button [OK].
                                        8 In menu Partial Conditions, open Add Part.Cond. (AND). A new element
                                          condition appears, and can be configured.
                                        9 Open the combo box (by default showing Only Formula 1) and select >=
                                          (greater or equal).
                                        10 Activate the radio button Value. The dialog Enter Value (Numeric) automat-
                                           ically appears. Since the new rack shall only contain lites over 1,20, acti-
                                           vate the radio button Length, and enter in section New Value 1200 mm.
                                           Close the dialog via button [OK] This value will appear in the bottom field
                                           of the condition.
                                        11 Click on the top input field of the condition. The dialog Select Formulas --
                                           1-- appears automatically. Define what the value entered in the second in-
                                           put field shall refer to.
                                        12 Press button [New Formula …]. The dialog Formula Editor appears. Enter
                                           a characteristic name for the formula in the top left field. Example: Large
                                           Dimension.
                                            Software Reference, “Top input field” on page R-67
                                        13 In section Existing Properties, double-click on Large_Dim.
                                            Software Reference, “Existing Properties” on page R-68
                                        14 Close the dialog via button [OK] You will find yourself back in dialog Condi-
                                           tion Editor.
1.02 / 01-2017




                 A+W Production Formula Editor                                                                    R-29
                 Conditions for Racks                                                                           Operation




                                           The defined condition looks like this:




                                           Fig. R-15     Condition Rack for lites >= 1200 mm


                                           Close the dialog via menu Conditions > OK, or by clicking on           .
                                           You will find yourself back in dialog Select Conditions --1--. You will find the
                                           defined condition Large Lite at the end of the list Existing Properties.


                                         This is how to allocate a condition to a rack
                                        1 Open the Organization Dialog via
                                           Master Data > Detailed Scheduling> Organization
                                        2 Open tab Production Sequence.
                                        3 Tag the rack the condition shall be allocated to.
                                        4 Press button [New Condition]. The dialog Select Conditions --1-- appears.
                                        5 On the list of Existing Conditions, tag the condition to be allocated to this
                                          rack.
                                        6 Close the dialog via button [OK].
                                        7 The condition was added to the rack tagged in tab Production Sequence.


                                         How to delete a condition allocated to a rack
                                        1 Open the Organization Dialog via
                                           Master Data > Detailed Scheduling> Organization
                                        2 Open tab Production Sequence.
                                        3 Double-click on the rack to open it.
                                        4 Tag the condition to be deleted.
                                        5 Press the [Delete] button. The condition will be deleted instantly.

                                           Delete
                                           Deletion is not accompanied by a security check. If you have deleted some-
                                           thing by mistake, leave the tab Production Sequence via button [Cancel].
                                           The system will want to know whether the changes shall be ignored. An-
1.02 / 01-2017




                                           swer [OK]. The Organization Dialog will be closed. When you open it next,
                                           the data will still be there.




                 R-30                                                                   A+W Production Formula Editor
                 Operation                                                         Conditions for Organization Groups




                                        Conditions for Organization
                                        Groups
                                        Explains how to define, change, or delete conditions for organization groups
                                        in section Organization.


                                         How to define a condition for an organization group, filtering IG with
                                          Grills for a second production step
                                        1 Open the Organization Dialog via
                                           Master Data > Detailed Scheduling> Organization
                                        2 Open tab Production Sequence.
                                        3 Tag the rack for which you want to define an organization group.
                                        4 Press button [New Condition]. The dialog Select Conditions --1-- appears.
                                            Software Reference, “Select Conditions” on page R-46
                                        5 Press button [New Condition …]. This opens the dialog Conditions Editor.
                                            Software Reference, “Conditions - Editor” on page R-48
                                        6 In menu Conditions, open Names. This leads to dialog Condition Name
                                          Field New Name shows New Condition by default. Give the condition a
                                          characteristic name. In our example: IG – Grills. Close the dialog via but-
                                          ton [OK].
                                            Software Reference, “Condition Name” on page R-53
                                        7 In menu Conditions, open Info. This opens dialog Info. Enter a clear de-
                                          scription of this condition. In our example: Item was allocated to produc-
                                          tion step 2 MZO_ROUTE_MAP.ROUTE =2. Close the dialog via button
                                          [OK].
                                            Software Reference, “Info” on page R-54
                                        8 In menu Partial Conditions, open Add Part.Cond. (AND). A new element
                                          condition appears, and can be configured.
                                        9 Open the combo box (by default showing Only Formula 1) and select ==
                                          (equal).
                                        10 Activate the radio button Value. The dialog Enter Value (Numeric) automat-
                                           ically appears. Since IG with Grills only produced in production step 2, ac-
                                           tivate the radio button Digit and enter in section New Value 2. Close the
                                           dialog via button [OK]. This value will appear in the bottom field of the con-
                                           dition
                                            Software Reference, “Enter Value (Numeric)” on page R-55
                                        11 Click on the top input field of the condition. The dialog Select Formulas --
                                           1-- appears automatically. Define what the value entered in the second in-
                                           put field shall refer to.
1.02 / 01-2017




                                            Software Reference, “Select Formulas” on page R-64




                 A+W Production Formula Editor                                                                     R-31
                 Conditions for Organization Groups                                                              Operation




                                         12 Press button [New Formula …]. The dialog Formula Editor appears. Enter
                                            a characteristic name for the formula in the top left field. In our example:
                                            Production Step.
                                             Software Reference, “Top input field” on page R-67
                                         13 In section Existing Properties double-click on Route. Section Formula
                                            shows $Route.
                                             Software Reference, “Existing Properties” on page R-68
                                         14 Close the dialog via button [OK]. You will find yourself back in dialog Con-
                                            dition editor.
                                            The defined condition looks like this:




                                            Fig. R-16     Condition Production Step = 2


                                            Close the dialog via menu Conditions > OK, or by clicking on           .
                                            You will find yourself back in dialog Select Conditions --1--. You will find the
                                            defined condition IG - Grills at the end of the list Existing Properties.
                                         15 Tag the condition and press [Ok]. The condition will be added to the previ-
                                            ously tagged organization group.


                                          How to allocate an existing property to an organization group
                                         1 Open the Organization Dialog via
                                            Master Data > Detailed Scheduling> Organization
                                         2 Open tab Production Sequence.
                                         3 Tag the organization group to define a condition.
                                         4 Press button [New Condition]. The dialog Select Conditions --1-- appears.
                                         5 On the list of Existing Conditions, tag the condition to be allocated to this
                                           organization group.
                                         6 Close the dialog via button [OK].
                                         7 The condition was added to the organization group tagged in tab Produc-
                                           tion Sequence.
1.02 / 01-2017




                 R-32                                                                     A+W Production Formula Editor
                 Operation                                                        Conditions for Organization Groups




                                         How to delete a condition allocated to an organization group
                                        1 Open the Organization Dialog via
                                           Master Data > Detailed Scheduling> Organization
                                        2 Open tab Production Sequence.
                                        3 Double-click on the organization group to open it.
                                        4 Tag the condition to be deleted
                                        5 Press the [Delete] button. The condition will be deleted instantly.

                                           Delete
                                           Deletion is not accompanied by a security check. If you have deleted some-
                                           thing by mistake, leave the tab Production Sequence via button [Cancel].
                                           The system will want to know whether the changes shall be ignored. An-
                                           swer [OK]. The Organization Dialog will be closed. When you open it next,
                                           the data will still be there.
1.02 / 01-2017




                 A+W Production Formula Editor                                                                  R-33
                 Group Formation Mode                                                                         Operation




                                        Group Formation Mode
                                        This example serves to add another selectable mode for group formation for
                                        organization groups and racks.


                                         This is how you create a grouping by number of lites per customer,
                                          i.e. a group will be created per customer and this group will be sorted
                                          by the number of lites included. The group with the largest number of
                                          lites will be produced first.
                                        1 Open the Grouping/Sorting Dialog via
                                           Master Data > Detailed Scheduling> Grouping
                                        2 Press button [Formulas …]. The dialog Select Formulas --1-- appears.
                                        3 Press button [New Formula …]. The dialog Formula Editor appears.
                                        4 Enter the name for the grouping formula in the top left field. In our example,
                                          number of lites per customer.
                                        5 In section Existing Properties, double-click on Qty. Section Formula shows
                                          $Qty.
                                        6 Press button [Quantity …]. The dialog Select Quantity --1-- appears.
                                        7 Use button [New Quantity …] to define a new quantity. This opens dialog
                                          Quantity Editor. Starting from a given quantity we will perform quantity op-
                                          erations to get the final quantity. Detailed Scheduling transfers to the for-
                                          mula editor values for a customer's item, the quantity calculation, and all
                                          orders of the job on hand. Just add the customer number.
                                        8 In menu Quantity, open Names and enter a new, characteristic name for
                                          the quantity. In our example, number of lites per customer. Close the di-
                                          alog via button [OK].
                                        9 In menu Quantity, open Given Quantity. As a result, not only the item used
                                          to start the quantity editor will be considered for quantity calculation, but
                                          also all items of the job.
                                        10 As the required quantity shall not include all elements, but only the released
                                           elements, activate in dialog Quantity Editor the checkbox Master.
                                        11 To add the customer number as a property to the quantity, select in menu
                                           Quantity, Formula. The dialog Select Formulas --2-- appears. Use button
                                           [New Formula …] to enter the formula for the customer number. The dialog
                                           Formula Editor appears.
                                        12 Enter the formula name in the top left input field. In our example, Customer
                                           Number.
                                        13 In section Existing Properties, double-click on Customer No. Section For-
                                           mula shows $Customer No.
                                        14 Press [Ok]. You will return to dialog Select Formulas --2--. The last entry on
                                           the list will be the just defined formula for the customer number. Tag the
1.02 / 01-2017




                                           Customer No. on the list, and press [Ok]. This brings you back to dialog
                                           Quantity Editor.



                 R-34                                                                  A+W Production Formula Editor
                 Operation                                                                       Group Formation Mode




                                        15 The right side of the status line of the quantity editor shows whether - and
                                           if so, which - formula is used to define the new quantity. In our example, this
                                           is: Formula: Customer No.
                                        16 Tag all open dialogs via [Ok] until you reach dialog Grouping/Sorting.
                                        17 The list of formulas now includes the formula number of lites per customer.
                                           Tag the formula and press [Add]. The formula will be added to the group-
                                           ings in tab Grouping Editor. It will be available in the settings for the Orga-
                                           nization Groups and the Racks, in section Group Formation.
1.02 / 01-2017




                 A+W Production Formula Editor                                                                      R-35
                 Conditions for Production Sections                                                             Operation




                                          Conditions for Production
                                          Sections
                                          This tells you how to define, change, or delete conditions for production sec-
                                          tions in part Machinery Allocation.


                                           How to define a condition for a production section, filtering all lites
                                            with Grills
                                          1 Open dialog Production Sections via
                                             Master Data > Machinery Allocation > Setup
                                          2 Tag the production section for which you want to define a condition.
                                          3 Use the right mouse key. The context menu appears. From the context
                                            menu, select
                                             Condition of production section > New
                                          4 The dialog Select Conditions --1-- appears.
                                          5 Press button [New Condition …]. This opens the dialog Conditions Editor.
                                          6 In menu Conditions, open Names. This leads to dialog Condition Name.
                                            Field New Name shows New Condition by default. Give the condition a
                                            characteristic name. In our example: Grills - IG. Close the dialog via button
                                            [OK].
                                          7 In menu Conditions, open Info. This opens dialog Info. Enter a clear de-
                                            scription of this condition. Example: This condition is true if the item shows
                                            a Grill flag. Close the dialog via button [OK].
                                          8 In menu Partial Conditions, open Add Part.Cond. (AND). A new element
                                            condition appears, and can be configured.
                                          9 The combo box shows Only Formula 1 by default. In our example, this re-
                                            mains unchanged.
                                          10 The radio button Normal is active by default. In our example, this remains
                                             unchanged, too.
                                          11 Click on the top input field of the condition. The dialog Select Formulas --
                                             1-- appears automatically.
                                          12 Press button [New Formula …]. The dialog Formula Editor appears. Enter
                                             a characteristic name for the formula in the top left field. In our example:
                                             Grills
                                              Software Reference, “Top input field” on page R-67
                                          13 In section Existing Properties double-click on Item_Grill_Flag. Section For-
                                             mula shows $Item_Grill_Flag
                                              Software Reference, “Existing Properties” on page R-68
1.02 / 01-2017




                                          14 Close the dialog via button [OK]. This brings you to dialog Select Formulas
                                             --1--. The just defined formula is tagged already.



                 R-36                                                                   A+W Production Formula Editor
                 Operation                                                           Conditions for Production Sections




                                        15 Close the dialog via button [OK].You will find yourself back in dialog Condi-
                                           tion Editor.
                                           The defined condition looks like this:




                                           Fig. R-17     Condition IG with Grills


                                           Close the dialog via menu Conditions > OK, or by clicking on           .
                                           You will find yourself back in dialog Select Conditions --1--. You will find the
                                           defined condition Grills - IG at the end of the list Existing Properties.


                                         This is how to allocate a condition to a production section
                                        1 Open dialog Production Section via
                                           Master Data > Machinery Allocation > Setup
                                        2 Tag the production section the condition shall be allocated to.
                                        3 Use the right mouse key. The context menu appears. From the context
                                          menu, select
                                           Condition for Production Section > New
                                        4 The dialog Select Conditions --1-- appears.
                                        5 On the list of Existing Conditions, tag the condition to be allocated to this
                                          production section.
                                        6 Close the dialog via button [OK].
                                        7 The condition was added to the tagged production section.
1.02 / 01-2017




                 A+W Production Formula Editor                                                                        R-37
                 Conditions for Production Sections                                                          Operation




                                           How to delete a condition allocated to a production section
                                          1 Open dialog Production Section via
                                             Master Data > Machinery Allocation > Setup
                                          2 Double-click on the production section to open it.
                                          3 Tag the condition to be deleted.
                                          4 Use the right mouse key. The context menu appears. From the context
                                            menu, select Delete Condition.
                                             The condition will be deleted instantly!

                                             Delete
                                             Deletion is not accompanied by a security check. If you have deleted some-
                                             thing by mistake, leave the tab Production Sections via button [Cancel].
                                             When you open it next, the data will still be there.
1.02 / 01-2017




                 R-38                                                                   A+W Production Formula Editor
                 Operation                                                                                                      More Examples




                                        More Examples
                                         How to define a condition for toughened glass within IG, or float glass
                                          processing
                                        1 First step




                                           Fig. R-18


                                           In formula Toughened Glass, the property E_TG is returned
                                        2 Now check whether the element is part of IG



                                                              1. Elementary Condition         2. General Quantity Description for Mate
                                                              including Property PT_TGH




                                           3. Composite Start Quantity


                                                                                                   4. Minus or Reduction Size




                                           The quantity operation begins with the start quantity
                                           and searchs child parts of all parents, substract
                                           afterwards itself. Final quantity is remaining mates.



                                        3 As an element cannot be toughened glass and IG at the same time, the
                                          condition shown in step 2 cannot work. Hence …
1.02 / 01-2017




                 A+W Production Formula Editor                                                                                           R-39
                 More Examples                                                                        Operation




                                    Fig. R-19


                                 4 Check the Or connection, whether one of the sub-elements is a processing
                                   step. Another condition will be created, checking the formula Processing
                                   for all childs.




                                    Fig. R-20


                                  The processing steps directly below
                                 1 The final quantity shall contain only the processing steps below the start el-
                                   ement which will be made after the last processing steps defined.
                                 2 The system first unites all sub-elements which are no processings.
                                 3 Quantity Defined processing steps below = { ; ANYCHILD ; condition is
                                   no processing ; }
                                 4 This quantity is used to define the number of elements and processing
                                   steps below the start element you do not require.
1.02 / 01-2017




                                 5 Quantity Unwanted elements/processing steps below = { number of de-
                                   fined processing steps below ; ANYCHILD+SELF ; ; }




                 R-40                                                          A+W Production Formula Editor
                 Operation                                                                           More Examples




                                        6 The required quantity is determined by the number of all sub-elements
                                          and the number of unwanted elements/processing steps below.
                                                 { number of all sub-elements - number of unwanted elements/process-
                                                 ings below ; SELF ; ; }
1.02 / 01-2017




                 A+W Production Formula Editor                                                                R-41
                 More Examples                       Operation
1.02 / 01-2017




                 R-42            A+W Production Formula Editor
Formula Editor                  R

                 Software Reference




                 A+W Production
                 Software Reference                                                                      Formula Editor




                                        Formula Editor
                                        The Formula Editor is used in the following areas of A+W Production:
                                        •   Organization
                                        •   Machinery Allocation
                                        •   Labels, Sketches, Bender text
                                        Instructions on how to open individual dialogs are provided in the following di-
                                        alog descriptions. If there exist alternative methods to open a dialog, these are
                                        also specified.
1.02 / 01-2017




                 A+W Production Formula Editor                                                                     R-45
                 Formula Editor                                                              Software Reference




                                  Select Conditions
                                  Load via

                                  Organization
                                  Master Data > Detailed Scheduling > Organization > Tab: Production Se-
                                  quence > Tag Organization Group > [New Condition]
                                  Master Data > Detailed Scheduling > Organization > Tab: Production Se-
                                  quence > Tag Rack > [New Condition]

                                  Machinery Allocation
                                  Master Data > Machinery Allocation > Setup > Tag Production Section > right
                                  mouse key > Condition of Production Section > New
                                  Master Data > Machinery Allocation > Setup > Tag Condition of Production
                                  Section > right mouse key > Edit Condition
                                  Master Data > Machinery Allocation > Setup > [Technology] > [New] > [New]
                                  Master Data > Machinery Allocation > Setup > [Technology] > [Change] >
                                  [New]/[Edit]

                                  Labels, Sketches, Bender Text
                                  Master Data > Labels / Sketches / Bender texts > Configuration … > Tag Con-
                                  dition > [Formula Editor]




                                  Fig. R-21    Select Conditions --1--


                                  This dialog allows to select, or change existing conditions for the sections Or-
                                  ganization, Machinery Allocation and Labels, Sketches, Bender text, or to de-
                                  fine new conditions.

                                  Fields
1.02 / 01-2017




                                  Existing Conditions The table lists all conditions existing in the system for
                                  the sections Organization, Machinery Allocation and Labels, Sketches, Bend-
                                  er text. The contents differ from section to section!



                 R-46                                                           A+W Production Formula Editor
                 Software Reference                                                                         Formula Editor




                                        No Condition If this checkbox is active, the dialog shows as a result that
                                        Nothing was selected.

                                        Description The field contains a detailed description of the condition. This is
                                        the text entered in field Info.
                                         Software Reference, “Info” on page R-54

                                        Buttons

                                        Delete Use this button to delete the tagged condition. Deletion will be made
                                        without a security check. Should you delete something by mistake, just return
                                        to the original dialog (organization dialog, label dialog, sketch type dialog,
                                        bender text type dialog, machinery allocation dialog). When you close this via
                                        [Abort] , the system will ask you whether or not the amendments shall be ig-
                                        nored.

                                        New Condition Press this button to open dialog Conditions - Editor. You can
                                        define a new condition.
                                         Software Reference, “Conditions - Editor” on page R-48

                                        Edit Press this button to open dialog Conditions - Editor for the tagged condi-
                                        tion.
                                         Software Reference, “Conditions - Editor” on page R-48


                                        Additional information on conditions
                                         Functional Principle, “Elements of the Formula Editor: Level I” on page R-9
                                         Functional Principle, “Elements of the Formula Editor: Level II” on page R-15
1.02 / 01-2017




                 A+W Production Formula Editor                                                                        R-47
                 Formula Editor                                                            Software Reference




                                  Conditions - Editor
                                  Load via

                                  Organization
                                  Master Data > Detailed Scheduling > Organization > Tab: Production Se-
                                  quence > Tag Organization Group > [New Condition] > [New Condition …] /
                                  [Edit]
                                  Master Data > Detailed Scheduling > Organization > Tab: Production Se-
                                  quence > Tag Rack > [New Condition] > [New Condition …] / [Edit]

                                  Machinery Allocation
                                  Master Data > Machinery Allocation > Setup > Tag Production Section > right
                                  mouse key > Condition of Production Section > New > [New Condition …] /
                                  [Edit]
                                  Master Data > Machinery Allocation > Setup > Tag Condition of Production
                                  Section > right mouse key > Edit Condition > [New Condition …] / [Edit]

                                  Labels, Sketches, Bender text
                                  Master Data > Labels / Sketches / Bender text > Configuration … > Tag Con-
                                  dition > [Formula Editor] > [New Condition …] / [Edit]




                                  Fig. R-22   Conditions - Editor


                                  Conditions - Editor allows to change a tagged condition, or to define a new
                                  condition.
1.02 / 01-2017




                 R-48                                                         A+W Production Formula Editor
                 Software Reference                                                                        Formula Editor




                                        The following table lists the dialogs and functions offered in the menus Condi-
                                        tions and Partial Conditions.

                                        Menu Entry                   Dialog/Function

                                        Menu Conditions:
                                        Name                          “Condition Name” on page R-53
                                        Info                          “Info” on page R-54
                                        Quantity                      “Select Quantity” on page R-57

                                        Invert                        “Invert” on page R-54

                                        Transferred quantity          “Given Quantity” on page R-55

                                        OK                            Tab. on page R-49

                                        Abort                         Tab. on page R-49

                                        Menu Element
                                        Conditions:
                                                                      Tab. on page R-49
                                         Add (column)

                                        Add (line)                    Tab. on page R-49

                                        Delete                        Tab. on page R-50

                                        Tab. R-2     List of Dialogs in Menus Conditions and Partial Conditions

                                        Instructions on how to open individual dialogs are provided in the following di-
                                        alog descriptions. If there are several ways of loading a dialog, these will be
                                        listed as well.

                                        Tool Bar

                                        Tool         Explanation

                                                     The defined condition will be saved, and the
                                                     editor is closed

                                                     The defined condition will be rejected, and the
                                                     editor is closed

                                                     Opens the window to define the condition.
                                                     Double-click to open two windows next to
                                                     another; these represent an And connection.
                                                      Software Reference, “Condition” on
                                                       page R-51

                                                     Opens the window to define the condition.
                                                     Double-click to open two windows, one below
                                                     the other; these represent an Or connection.
1.02 / 01-2017




                                                      “Condition” on page R-51

                                        Tab. R-3     Tool Bar for the Definition of Conditions



                 A+W Production Formula Editor                                                                     R-49
                 Formula Editor                                                                 Software Reference




                                  Tool          Explanation

                                                Deletes the selected condition.

                                  Tab. R-3      Tool Bar for the Definition of Conditions

                                  Radio Buttons

                                  All Considers the conditions for all elements of a BOM. With this setting, a lite
                                  without pattern - for instance - will be allocated to a rack with the condition pat-
                                  tern if the mate is patterned.

                                  One Only the characteristics of the lite in question will be considered.

                                  Null The quantity allocated to the condition will not be taken into account.
1.02 / 01-2017




                 R-50                                                               A+W Production Formula Editor
                 Software Reference                                                                    Formula Editor




                                        Condition
                                        Load via

                                        Organization
                                        Master Data > Detailed Scheduling > Organization > Tab: Production Se-
                                        quence > Tag Organization Group > [New Condition] > [New Condition] >
                                        Menu Partial Conditions > Add …
                                        Master Data > Detailed Scheduling > Organization > Tab: Production Se-
                                        quence > Tag Rack > [New Condition] > [New Condition] > Menu Partial Con-
                                        ditions > Add …

                                        Machinery Allocation
                                        Master Data > Machinery Allocation > Setup > Tag Production Section > right
                                        mouse key > Condition of Production Section> New > [New Condition …] >
                                        Menu Partial Conditions > Add …
                                        Master Data > Machinery Allocation > Setup > Tag Condition of Production
                                        Section > right mouse key > Edit Condition > [New Condition …] > Menu Par-
                                        tial Conditions > Add …

                                        Labels, Sketches, Bender Text
                                        Master Data > Labels / Sketches / Bender text > Configuration … > Tag Con-
                                        dition > [Formula Editor] > [New Condition …] > Menu Partial Conditions >
                                        Add …




                                        Fig. R-23    Condition


                                        Top Input field Click on the field to open the dialog Select Formulas. You can
                                        select an existing formula, or enter a new one.
                                         Software Reference, “Select Formulas” on page R-64
1.02 / 01-2017




                 A+W Production Formula Editor                                                                  R-51
                 Formula Editor                                                                Software Reference




                                  Central Selection Field Open the combo box and select the operator. Valid
                                  entries:
                                  • Only Formula 1
                                  • == equal
                                  • == unequal
                                  • < smaller
                                  • <= smaller or equal
                                  • > bigger
                                  • >= bigger or equal

                                  Bottom Input Field Click on the field to open dialog Select Formulas, dialog
                                  Enter Value (Numeric) or dialog Select Conditions. The active radio button
                                  (Normal, Value, Conditions) defines which dialog is going to be opened. If ra-
                                  dio button Normal is active, dialog Select Formulas appears. You can select
                                  an existing formula, or enter a new one. If radio button Value is active, dialog
                                  Enter Value (Numeric) appears. Enter the required value. If radio button Con-
                                  ditions is active, dialog Select Conditions will be opened. You can select an ex-
                                  isting formula, or enter a new one.
                                   Software Reference, “Select Formulas” on page R-64
                                   Software Reference, “Enter Value (Numeric)” on page R-55
                                   Software Reference, “Select Conditions” on page R-46

                                  Normal Activate the radio button, then click on the bottom input field to open
                                  the dialog Select Formulas.
                                   Software Reference, “Select Formulas” on page R-64

                                  Value Activate this radio button to open dialog Enter Value (Numeric).
                                   Software Reference, “Enter Value (Numeric)” on page R-55

                                  Conditions Activate the radio button, then click on the bottom input field to
                                  open dialog Selection Conditions --2 --.


                                  Additional information on the condition
                                   “Elements of the Formula Editor: Level I” on page R-9
                                   “Elements of the Formula Editor: Level II” on page R-15
1.02 / 01-2017




                 R-52                                                            A+W Production Formula Editor
                 Software Reference                                                                   Formula Editor




                                        Condition Name
                                        Load via

                                        Organization
                                        Master Data > Detailed Scheduling > Organization > Tab: Production Se-
                                        quence > Tag Organization Group > [New Condition] > [New Condition …] >
                                        Menu Conditions > Name
                                        Master Data > Detailed Scheduling > Organization > Tab: Production Se-
                                        quence > Tag Rack > [New Condition] > [New Condition …] > Menu Condi-
                                        tions > Name

                                        Machinery Allocation
                                        Master Data > Machinery Allocation > Setup > Tag Production Section > right
                                        mouse key > Condition of Production Section > New > [New Condition …] >
                                        Menu Conditions > Name
                                        Master Data > Machinery Allocation > Setup > Open Production Section > Tag
                                        Existing Condition > right mouse key > Edit Condition > [New Condition …] >
                                        Menu Conditions > Name

                                        Labels, sketches, bender text
                                        Master Data > Labels / Sketches / Bender text > Configuration … > Tag Con-
                                        dition > [Formula Editor] > [New Condition …] > Menu Conditions > Name




                                        Fig. R-24   Condition Name


                                        Give the conditions characteristic names. The name will be shown in the sta-
                                        tus line of dialog Conditions - Editor.

                                        Fields

                                        Old Name If a condition was given no name so far, this field will read new
                                        condition by default. When a name was allocated, this will be shown as in the
                                        above example >2300.

                                        New Name Enter the name of the condition. This can be overridden at any
                                        time. The defined name appears in the status line of Conditions - Editor.
1.02 / 01-2017




                 A+W Production Formula Editor                                                                 R-53
                 Formula Editor                                                                  Software Reference




                                  Info
                                  Load via

                                  Organization
                                  Master Data > Detailed Scheduling > Organization > Tab: Production Se-
                                  quence > Tag Organization Group > [New Condition] [New Condition …] >
                                  Menu Conditions > Info
                                  Master Data > Detailed Scheduling > Organization > Tab: Production Se-
                                  quence > Tag Rack > [New Condition] > [New Condition …] > Menu Condi-
                                  tions > Info

                                  Machinery Allocation
                                  Master Data > Machinery Allocation > Setup > Tag Production Section > right
                                  mouse key > Condition of Production Section > New > [New Condition …] >
                                  Menu Conditions > Info
                                  Master Data > Machinery Allocation > Setup > Open Production Section > Tag
                                  Existing Condition > right mouse key > Edit Condition > [New Condition …] >
                                  Menu Conditions > Info

                                  Labels, Sketches, Bender Text
                                  Master Data > Labels / Sketches / Bender text > Configuration … > Tag Con-
                                  dition > [Formula Editor] > [New Condition …] > Menu Conditions > Info




                                  Fig. R-25     Condition Information


                                  You can describe the condition. The text will appear in dialog Select Condi-
                                  tions in section Description.


                                  Invert
                                  A condition can be inverted, i.e. it is fulfilled if the result of the comparisons is
                                  not fulfilled, and vice versa. This way, you can easily create from an existing
                                  condition the inverted one. The inverted condition contains just one compari-
                                  son which will be allocated the original condition. Moreover, the characteristic
                                  invert will be selected for the inverted condition. The status line shows INV in
                                  front of the condition name.
                                  This menu can be enabled or disabled as required.
1.02 / 01-2017




                 R-54                                                              A+W Production Formula Editor
                 Software Reference                                                                     Formula Editor




                                        Given Quantity
                                        This menu can be enabled or disabled as required. If it is active, the system
                                        will not only consider the item by which the dialog Conditions - Editor was
                                        opened, but also all items of the job when determining the quantities.


                                        Enter Value (Numeric)
                                        Load via

                                        Organization
                                        Master Data > Detailed Scheduling > Organization > Tab: Production Se-
                                        quence > Tag Organization Group > [New Condition] > [New Condition …] >
                                        Menu Partial Conditions > Add > Activate Radio Button [Value]
                                        Master Data > Detailed Scheduling > Organization > Tab: Production Se-
                                        quence > Tag Rack > [New Condition] > [New Condition …] > Menu Partial
                                        Conditions > Add > > Activate Radio Button [Value]

                                        Machinery Allocation
                                        Master Data > Machinery Allocation > Setup > Tag Production Section > right
                                        mouse key > Condition of Production Section > New > [New Condition …] >
                                        Menu Partial Conditions > Add > Activate Radio Button [Value]
                                        Master Data > Machinery Allocation > Setup > Open Production Section > Tag
                                        Existing Condition > right mouse key > Edit Condition > [New Condition …] >
                                        Menu Partial Conditions > Add > Activate Radio Button [Value]

                                        Labels, Sketches, Bender Text
                                        Master Data > Labels / Sketches / Bender text > Configuration … > Labels /
                                        Sketches / Tag Bender Text > [Formula Editor] > [New Condition …] > Menu
                                        Partial Conditions > Add > Activate Radio Button [Value]




                                        Fig. R-26    EnterValue (Numeric)


                                        This dialog is used to enter numerical values. Activate the appropriate radio
                                        button to specify whether the numerical value is Digit, Thickness, Text, Length
                                        or Airspace.
1.02 / 01-2017




                 A+W Production Formula Editor                                                                   R-55
                 Formula Editor                                                                 Software Reference




                                  Fields

                                  Old Value If a condition was given no value so far, this field will read 0 by de-
                                  fault. If a value was allocated, this will be shown.

                                  New Value Enter the value for the condition. This can be overridden at any
                                  time.

                                  Radio Buttons

                                  Digit If the condition refers to a quantity for instance, activate this radio but-
                                  ton; in field New Value enter the corresponding Digit. Example:
                                  • Quantity > 10
                                  • Glass type = 1700

                                  Thickness If this condition refers to Thickness, activate this radio button; in
                                  field New Value enter the corresponding Thickness in mm.

                                  Text If this condition refers to Text, activate this radio button; in field New Val-
                                  ue enter the corresponding Text.

                                  Length If the condition refers to a length, activate this radio button; in field
                                  New Value enter the corresponding Length.

                                  Airspace If the condition refers to an airspace, activate this radio button; in
                                  field New Value enter the corresponding Airspace.
1.02 / 01-2017




                 R-56                                                             A+W Production Formula Editor
                 Software Reference                                                                         Formula Editor




                                        Select Quantity
                                        Load via

                                        Organization
                                        Master Data > Detailed Scheduling > Organization > Tab: Production Se-
                                        quence > Tag Organization Group > [New Condition] > [New Condition …] >
                                        Menu Partial Conditions > Add > click on the first input field of the partial con-
                                        dition > [New Formula …] > [Quantity …]
                                        Master Data > Detailed Scheduling > Organization > Tab: Production Se-
                                        quence > Tag Rack > [New Condition] > [New Condition …] > Menu Partial
                                        Conditions > Add > click on the first input field of the partial condition > [New
                                        Formula …] > [Quantity …]

                                        Machinery Allocation
                                        Master Data > Machinery Allocation > Setup > Tag Production Section > right
                                        mouse key > Condition of Production Section > New > [New Condition …] >
                                        Menu Partial Conditions > Add > click on the first input field of the partial con-
                                        dition > [New Formula …] > [Quantity …]
                                        Master Data > Machinery Allocation > Setup > Open Production Section > Tag
                                        Existing Condition > right mouse key > Edit Condition > [New Condition …] >
                                        Menu Partial Conditions > Add > click on the first input field for the partial con-
                                        dition > [New Formula ….] > [Quantity …]

                                        Labels, Sketches, Bender Text
                                        Master Data > Labels / Sketches / Bender text > Configuration … > Labels /
                                        Sketches / Tag Bender Text > [Formula Editor] > [New Condition …] > Menu
                                        Partial Conditions > Add > click on the first input field of the partial condition >
                                        [New Formula …] > [Quantity …]




                                        Fig. R-27     Select Quantity


                                        This dialog allows to select, or change existing conditions for the sections Or-
1.02 / 01-2017




                                        ganization, Machinery Allocation and Labels, Sketches, Bender text, or to de-
                                        fine new conditions.



                 A+W Production Formula Editor                                                                        R-57
                 Formula Editor                                                             Software Reference




                                  Fields

                                  Existing Quantities The table lists all conditions existing in the system for
                                  the sections Organization, Machinery Allocation and Labels, Sketches, Bend-
                                  er text. The contents differ from section to section!

                                  No Quantity If this checkbox is active, the dialog shows as a result that Noth-
                                  ing was selected.

                                  Description The field contains a detailed description of the quantity. This is
                                  the text entered in field Info.
                                   Software Reference, “Info” on page R-54

                                  Buttons

                                  Delete Use this button to delete the tagged quantity. Deletion will be made
                                  without a security check. Should you delete something by mistake, just return
                                  to the original dialog (organization dialog, label dialog, sketch type dialog,
                                  bender text type dialog, machinery allocation dialog). When you close this via
                                  [Cancel] , the system will ask you whether or not the amendments shall be ig-
                                  nored.

                                  New Quantity Press this button to open dialog Quantity Editor. You can de-
                                  fine a new quantity.
                                   Software Reference, “Quantity Editor” on page R-59

                                  Edit Press this button to open dialog Quantity Editor for the tagged quantity.
                                   Software Reference, “Quantity Editor” on page R-59
1.02 / 01-2017




                 R-58                                                           A+W Production Formula Editor
                 Software Reference                                                                       Formula Editor




                                        Quantity Editor
                                        Load via

                                        Organization
                                        Master Data > Detailed Scheduling > Organization > Tab: Production Se-
                                        quence > Tag Organization Group > [New Condition] > [New Condition …] >
                                        Menu Partial Conditions > Add > click on the first input field of the partial con-
                                        dition > [New Formula …] > [Quantity …] > [New Quantity …] / [Edit]
                                        Master Data > Detailed Scheduling > Organization > Tab: Production Se-
                                        quence > Tag Rack > [New Condition] > [New Condition …] > Menu Partial
                                        Conditions > Add > click on the first input field of the partial condition > [New
                                        Formula …] > [Quantity …] > [New Quantity …] / [Edit]

                                        Machinery Allocation
                                        Master Data > Machinery Allocation > Setup > Tag Production Section > right
                                        mouse key > Condition of Production Section > New > [New Condition …] >
                                        Menu Partial Conditions > Add > click on the first input field of the partial con-
                                        dition > [New Formula …] > [Quantity …] > [New Quantity …] / [Edit]
                                        Master Data > Machinery Allocation > Setup > Open Production Section > Tag
                                        existing condition > right mouse key > Edit Condition > [New Condition …] >
                                        Menu Partial Conditions > Add > click on the first input field of the partial con-
                                        dition > [New Formula …] > [Quantity …] > [New Quantity …] / [Edit]

                                        Labels, Sketches, Bender Text
                                        Master Data > Labels / Sketches / Bender text > Configuration … > Labels /
                                        Sketches / Tag bender text > [Formula Editor] > [New Condition …] > Menu
                                        Partial Conditions > Add > click on the first input field of the element condition
                                        > [New Formula …] > [Quantity …] > [New Quantity …] / [Edit]
1.02 / 01-2017




                                        Fig. R-28    Quantity - Editor


                                        Quantity Editor allows to change a tagged quantity, or to define a new quantity.



                 A+W Production Formula Editor                                                                      R-59
                 Formula Editor                                                                  Software Reference




                                  The following table gives an overview of the dialogs and functions available in
                                  the menus Quantity and Partial Quantities.

                                  Menu Entry                   Dialog/Function

                                  Menu Quantity:
                                  Name                          “Quantity Name” on page R-61
                                  Info                          “Info” on page R-63
                                  Condition                     “Select Conditions” on page R-46

                                  Formula                       “Select Formulas” on page R-64

                                  OK                            Tab. on page R-60

                                  Cancel                        Tab. on page R-60

                                  Menu Partial Quantities:
                                  Add Part. Cond.(AND)          Tab. on page R-60

                                  Add Part. Cond.(OR)           Tab. on page R-60

                                  Remove                        Tab. on page R-60

                                  Change                        Tab. on page R-61

                                  Tab. R-4     List of Dialogs in Menus Quantity and Partial Quantities

                                  Instructions on how to open individual dialogs are provided in the following di-
                                  alog descriptions. If there are several ways of loading a dialog, these will be
                                  listed as well.

                                  Tool Bar

                                  Tool         Explanation

                                               The defined quantity will be saved; the editor
                                               will be closed.

                                               The defined quantity will be rejected while the
                                               editor is closed.

                                               Opens the window to define the quantity.
                                               Double-click to open two windows next to
                                               another; these represent an And connection.

                                               Opens the window to define the quantity.
                                               Double-click to open two windows, one below
                                               the other; these represent an Or connection.
                                                “Condition” on page R-51

                                               Deletes the selected quantity.
1.02 / 01-2017




                                  Tab. R-5     Quantity Creator's Tool Bar




                 R-60                                                              A+W Production Formula Editor
                 Software Reference                                                                         Formula Editor




                                        Tool          Explanation

                                                      Switches between the first and the second
                                                      window.

                                        Tab. R-5      Quantity Creator's Tool Bar

                                        Checkboxes

                                        All All parts of the BOM containing the start part.

                                        Master The top part of the BOM (header) containing the start part.

                                        Parent Part right above the start part in the BOM.

                                        Self Start part.

                                        Child All direct sub-parts of the start part.

                                        Anychild All sub-parts of the start part, even the indirect ones.

                                        Bottom All basic parts below the start part.

                                        Up Up means that the final quantity consists of just one part. Starting from the
                                        start part, all main part of the start part will be checked whether they fulfil the
                                        condition. The final quantity contains the last part fulfilling the condition.
                                        Should one part fail to fulfil the condition, the upwards iteration will be aborted.

                                        AddUp AddUp means that the final quantity can consist of more than one
                                        part. Like with Up, there is an upward iteration from the start part which will be
                                        stopped if one part fails to fulfil the condition. The final quantity, however, con-
                                        tains all parts fulfilling the condition.


                                        Further information
                                         Functional Principle, “Elements of the Formula Editor: Level III” on page R-18



                                        Quantity Name
                                        Load via

                                        Organization
                                        Master Data > Detailed Scheduling > Organization > Tab: Production Se-
                                        quence > Tag Organization Group > [New Condition] > [New Condition …] >
                                        Menu Partial Conditions > Add > click on the first input field of the partial con-
                                        dition > [New Formula …] > [Quantity …] > [New Quantity …] / [Edit] > Menu
                                        Quantity > Name
1.02 / 01-2017




                                        Master Data > Detailed Scheduling > Organization > Tab: Production Se-
                                        quence > Tag Rack > [New Condition] > [New Condition …] > Menu Partial
                                        Conditions > Add > click on the first input field of the partial condition > [New



                 A+W Production Formula Editor                                                                        R-61
                 Formula Editor                                                               Software Reference




                                  Formula …] > [Quantity …] > [New Quantity …] / [Edit] > Menu Quantity >
                                  Name

                                  Machinery Allocation
                                  Master Data > Machinery Allocation > Setup > Tag Production Section > right
                                  mouse key > Condition of Production Section > New > [New Condition …] >
                                  Menu Partial Conditions > Add > click on the first input field of the partial con-
                                  dition > [New Formula …] > [Quantity …] > [New Quantity …] / [Edit] > Menu
                                  Quantity > Name
                                  Master Data > Machinery Allocation > Setup > Open Production Section > Tag
                                  existing condition > right mouse key > Edit Condition > [New Condition …] >
                                  Menu Partial Conditions > Add > click on the first input field of the partial con-
                                  dition > [New Formula …] > [Quantity …] > [New Quantity …] / [Edit] > Menu
                                  Quantity > Name

                                  Labels, Sketches, Bender Text
                                  Master Data > Labels / Sketches / Bender text > Configuration … > Labels /
                                  Sketches / Tag bender text > [Formula Editor] > [New Condition …] > Menu
                                  Partial Conditions > Add > click on the first input field of the element condition
                                  > [New Formula …] > [Quantity …] > [New Quantity …] / [Edit] > Menu Quan-
                                  tity > Name




                                  Fig. R-29    Quantity Name


                                  Give a characteristic name to the quantity. The name will be shown in the sta-
                                  tus line of dialog Quantity Editor.

                                  Fields

                                  Old Name If a condition was given no name so far, this field will read New
                                  Quantity by default. When a name was allocated already, this field will read,
                                  as in the above example, 1, if width < height.

                                  New Name Enter the name of the condition. This can be overridden at any
                                  time. The defined name appears in the status line of Conditions - Editor.
1.02 / 01-2017




                 R-62                                                            A+W Production Formula Editor
                 Software Reference                                                                       Formula Editor




                                        Info
                                        Load via

                                        Organization
                                        Master Data > Detailed Scheduling > Organization > Tab: Production Se-
                                        quence > Tag Organization Group > [New Condition] > [New Condition …] >
                                        Menu Partial Conditions > Add > click on the first input field of the partial con-
                                        dition > [New Formula …] > [Quantity …] > [New Quantity …] / [Edit] > Menu
                                        Quantity > Info
                                        Master Data > Detailed Scheduling > Organization > Tab: Production Se-
                                        quence > Tag Rack > [New Condition] > [New Condition …] > Menu Partial
                                        Conditions > Add > click on the first input field of the partial condition > [New
                                        Formula …] > [Quantity …] > [New Quantity …] / [Edit] > Menu Quantity > Info

                                        Machinery Allocation
                                        Master Data > Machinery Allocation > Setup > Tag Production Section > right
                                        mouse key > Condition of Production Section > New > [New Condition …] >
                                        Menu Partial Conditions > Add > click on the first input field of the partial con-
                                        dition > [New Formula …] > [Quantity …] > [New Quantity …] / [Edit] > Menu
                                        Quantity > Info
                                        Master Data > Machinery Allocation > Setup > Open Production Section > Tag
                                        existing condition > right mouse key > Edit Condition > [New Condition …] >
                                        Menu Partial Conditions > Add > click on the first input field of the partial con-
                                        dition > [New Formula …] > [Quantity …] > [New Quantity …] / [Edit] > Menu
                                        Quantity > Info

                                        Labels, Sketches, Bender Text
                                        Master Data > Labels / Sketches / Bender text > Configuration … > Labels /
                                        Sketches / Tag bender text > [Formula Editor] > [New Condition …] > Menu
                                        Partial Conditions > Add > click on the first input field of the element condition
                                        > [New Formula …] > [Quantity …] > [New Quantity …] / [Edit] > Menu Quan-
                                        tity > Info




                                        Fig. R-30    Info


                                        You can describe the condition. The text will appear in dialog Select Quantity
                                        in section Description.
1.02 / 01-2017




                 A+W Production Formula Editor                                                                      R-63
                 Formula Editor                                                               Software Reference




                                  Select Formulas
                                  Load via

                                  Organization
                                  Master Data > Detailed Scheduling > Organization > Tab: Production Se-
                                  quence > Tag Organization Group > [New Condition] > [New Condition …] >
                                  Menu Partial Conditions > Add > click on the first input field of the partial con-
                                  dition
                                  Master Data > Detailed Scheduling > Organization > Tab: Production Se-
                                  quence > Tag Rack > [New Condition] > [New Condition …] > Menu Partial
                                  Conditions > Add > click on the first input field of the partial condition

                                  Machinery Allocation
                                  Master Data > Machinery Allocation > Setup > Tag Production Section > right
                                  mouse key > Condition of Production Section > New > [New Condition …] >
                                  Menu Partial Conditions > Add > click on the first input field of the partial con-
                                  dition
                                  Master Data > Machinery Allocation > Setup > Open Production Section > Tag
                                  existing condition > right mouse key > Edit Condition > [New Condition …] >
                                  Menu Partial Conditions > Add > click on the first input field of the partial con-
                                  dition

                                  Labels, Sketches, Bender Text
                                  Master Data > Labels / Sketches / Bender text > Configuration … > Labels /
                                  Sketches / Tag bender text > [Formula Editor] > [New Condition …] > Menu
                                  Partial Conditions > Add > click on the first input field of the element condition




                                  Fig. R-31    Select Formulas


                                  This dialog allows to select, or change existing formulas for the sections Orga-
                                  nization, Machinery Allocation and Labels, Sketches, Bender text, or to define
                                  new formulas.
1.02 / 01-2017




                 R-64                                                            A+W Production Formula Editor
                 Software Reference                                                                         Formula Editor




                                        Fields

                                        Existing Formulas The table lists all formulas existing in the system for the
                                        sections Organization, Machinery Allocation and Labels, Sketches, Bender
                                        text.

                                        No Formula If this checkbox is active, the dialog shows as a result that Noth-
                                        ing was selected.

                                        Description The field contains a detailed description of the formula. This is
                                        the text entered in field Description.
                                         Software Reference, “Description” on page R-67

                                        Buttons

                                        Delete Use this button to delete the tagged formula. Deletion will be made
                                        without a security check. If you have deleted something by mistake, return to
                                        the original organization dialog. When you close this via [Cancel], the system
                                        will ask you whether or not the amendments shall be ignored.

                                        New Formula Press this button to open dialog Formula Editor. You can de-
                                        fine a new formula.
                                         Software Reference, “Formula Editor” on page R-66

                                        Edit Press this button to open dialog Formula Editor for the tagged formula.
                                         Software Reference, “Formula Editor” on page R-66


                                        More information on formulas
                                         Functional Principle, “Elements of the Formula Editor: Level I” on page R-9
                                         Functional Principle, “Elements of the Formula Editor: Level II” on page R-15
                                         Functional Principle, “Elements of the Formula Editor: Level III” on page R-18
1.02 / 01-2017




                 A+W Production Formula Editor                                                                        R-65
                 Formula Editor                                                                Software Reference




                                  Formula Editor
                                  Load via

                                  Organization
                                  Master Data > Detailed Scheduling > Organization > Tab: Production Se-
                                  quence > Tag Organization Group > [New Condition] > [New Condition …] >
                                  Menu Partial Conditions > Add > click on the first input field of the partial con-
                                  dition > [New Formula …]
                                  Master Data > Detailed Scheduling > Organization > Tab: Production Se-
                                  quence > Tag Rack > [New Condition] > [New Condition …] > Menu Partial
                                  Conditions > Add > click on the first input field of the partial condition > [New
                                  Formula …]

                                  Machinery Allocation
                                  Master Data > Machinery Allocation > Setup > Tag Production Section > right
                                  mouse key > Condition of Production Section > New > [New Condition …] >
                                  Menu Partial Conditions > Add > click on the first input field of the partial con-
                                  dition > [New Formula …]
                                  Master Data > Machinery Allocation > Setup > Open Production Section > Tag
                                  existing condition > right mouse key > Edit Condition > [New Condition …] >
                                  Menu Partial Conditions > Add > click on the first input field of the partial con-
                                  dition > [New Formula ….]

                                  Labels, Sketches, Bender Text
                                  Master Data > Labels / Sketches / Bender text > Configuration … > Labels /
                                  Sketches / Tag bender text > [Formula Editor] > [New Condition …] > Menu
                                  Partial Conditions > Add > click on the first input field of the element condition
                                  > [New Formula …]
1.02 / 01-2017




                                  Fig. R-32    Formula Editor




                 R-66                                                            A+W Production Formula Editor
                 Software Reference                                                                        Formula Editor




                                        This dialog allows to define new formulas. The simplest type of formula is just
                                        a field in the database. Section Existing Properties shows a list of the database
                                        fields. Tag one of the database fields to view the explanation on the field con-
                                        tents in the grey area below. You can of course define much more complex for-
                                        mulas by linking several fields, or using one or more of the existing forms.

                                        Fields

                                        Top input field Enter a characteristic name for the formula.

                                        Description Enter a detailed description of the formula.

                                        Formula Enter the database field required for the formula, i.e. select the ap-
                                        propriate database field in section Existing Properties, and double click on it.
                                        The database field will automatically be transferred to section Formula.

                                        Quantity Press this button to open dialog Select Quantity. You can select an
                                        existing quantity, or define a new one.
                                         Software Reference, “Select Quantity” on page R-57

                                        Given Quantity Checkbox If this checkbox is active, the system will consider
                                        all items of the batch for the quantity creation, not just the item by which the
                                        dialog Select Quantity was opened. The radio buttons in section Operation are
                                        active only if the checkbox is active as well.

                                        Radio buttons in section Operation
                                        The radio buttons in this section are active only if the checkbox Given Quantity
                                        is active, i.e. if a quantity was allocated to the formula. First, the formula will
                                        be analyzed for all parts of this quantity. The results of the formula will be pro-
                                        cessed as follows:

                                        Total (Value) Total results.

                                        Average Total/number of results.

                                        And Operation The results will be linked by a logical And.

                                        Or Operation The results will be linked by a logical Or.

                                           And/Or connections
                                           And/Or connections make sense only if the result of the formulas is 0 or 1!

                                        Minimum Smallest result.

                                        Maximum Biggest result.

                                        Number of Results Number of different results.
1.02 / 01-2017




                 A+W Production Formula Editor                                                                       R-67
                 Formula Editor                                                                 Software Reference




                                  Fields

                                  Existing Properties The table lists the database fields for sections Organiza-
                                  tion, Machinery Allocation and Labels, Sketches, Bender text. When a field is
                                  tagged, its contents will be described below.

                                     Existing properties
                                     Object properties within the organization are firmly linked for reasons for
                                     performance, and cannot be extended without program amendments. Ob-
                                     ject properties in connection with machinery allocation and labels can be
                                     flexibly extended via script DBInit.

                                  Existing Formulas The table lists all formulas existing in the system for the
                                  sections Organization, Machinery Allocation and Labels, Sketches, Bender
                                  text.


                                  Further information on the formula editor
                                   Functional Principle, “Elements of the Formula Editor: Level I” on page R-9
                                   Functional Principle, “Elements of the Formula Editor: Level II” on page R-15
                                   Functional Principle, “Elements of the Formula Editor: Level III” on page R-18
1.02 / 01-2017




                 R-68                                                              A+W Production Formula Editor
                 Software Reference                                                                      Formula Editor




                                        Select Allocation
                                        Master Data > Detailed Scheduling> Allocations




                                        Fig. R-33    Select Allocation


                                        This dialog allows to select or change allocations only for section Organiza-
                                        tion, or to define new allocations.

                                        Fields

                                        Existing Allocations The table lists all existing allocations in section Organi-
                                        zation.

                                        No Allocation If this checkbox is active, the dialog shows as a result that
                                        Nothing was selected.

                                        Description The field contains a detailed description of the allocation. This is
                                        the text entered in field Info.
                                         Software Reference, “Info” on page R-54

                                        Buttons

                                        Delete Use this button to delete the tagged allocation. Deletion will be made
                                        without a security check. Should you delete something by mistake, close the
                                        dialog via [Abort]. The changes will be ignored.

                                        New Allocation Press this button to open dialog Allocation Editor. You can
                                        define a new condition.
                                         Software Reference, “Allocation Editor” on page R-69

                                        Edit Press this button to open dialog Allocation Editor for the tagged alloca-
                                        tion.
                                         Software Reference, “Allocation Editor” on page R-69
1.02 / 01-2017




                                        Allocation Editor
                                        Master Data > Detailed Scheduling > Allocations > [New Allocation]


                 A+W Production Formula Editor                                                                    R-69
                 Formula Editor                                                                 Software Reference




                                  Fig. R-34     Allocation Editor


                                  Use this dialog to define a new allocation. The simplest type is the allocation
                                  of an object property to a formula. The result of the formula is allocated to the
                                  object property. The allocation can of course include a quantity. In this case,
                                  the result of the formula of the property will be allocated to all objects of the
                                  final quantity.

                                  Fields

                                  Top Input Field Give the allocation a characteristic name. When you open di-
                                  alog Allocation Editor via button [New Allocation], this field will read New Allo-
                                  cation by default. When you open the dialog via button [Edit], this field shows
                                  the name of the allocation you want to edit.

                                  Property When you open the combo box, the system shows the database
                                  fields that can be changed in connection with Detailed Scheduling. Select the
                                  required database field to view an explanation of the field contents in the grey
                                  area to the right of the combo box.

                                     Existing properties
                                     Object properties for Detailed Scheduling are firmly linked for reasons for
                                     performance, and cannot be extended without program amendments.

                                  Important allocations:
                                  • Stack width: Will be used for rack loads. Normally, this property represents
                                     the lite width.
                                  • Assessment: 100 by default. In connection with optimization, this serves to
                                     distribute lites to several stockplates. The smaller the value, the more lites
                                     will be shifted. This might help to avoid that in case of big lites, not all lites
                                     of a unit lie on the same stockplate.
                                  • Difference in thickness: Defines to what extent the glass thickness may
                                     change when lites are added.
                                  • Group number: 0 by default. If this group number is used to create produc-
                                     tion groups in Detailed Scheduling, this property must be allocated an ap-
                                     propriate formula first.
1.02 / 01-2017




                                  • Box: Freely disposable.
                                  • Extra thickness: 0 mm by default. Can be used to define that when stacking
                                     lites onto A racks, the system will consider lites thicker than determined by
                                     the glass thickness. This is frequently used for lites with silk screening.


                 R-70                                                              A+W Production Formula Editor
                 Software Reference                                                                         Formula Editor




                                           Each silk-screened lite can thus be protected by a piece of cardboard of X
                                           mm thickness. This value is allocated to the extra thickness. To make sure
                                           this is only applied to silk-screened lites, you have to enter the correct
                                           quantity.

                                        Formula Press this button to open dialog Select Formulas.
                                         Software Reference, “Select Formulas” on page R-64

                                        Field with grey background When you select a formula via button [Formu-
                                        la], this field shows the formula name.

                                        Quantity Press this button to open dialog Select Quantity. This does not only
                                        serve to allocate further parts (not only the actual one), but also to apply the
                                        allocation to certain parts.
                                         Software Reference, “Select Quantity” on page R-57

                                        Given Quantity Checkbox If this checkbox is active, the system will consider
                                        all items of the batch for the quantity creation, not just the item by which the
                                        dialog Select Quantity was opened.

                                        Field with grey background When you select a quantity via the [Quantity]
                                        button, this field shows the quantity name.


                                        Additional information on the allocation
                                         Functional Principle, “Elements of the Formula Editor: Level I” on page R-9
                                         Functional Principle, “Elements of the Formula Editor: Level II” on page R-15
1.02 / 01-2017




                 A+W Production Formula Editor                                                                        R-71
                 Formula Editor              Software Reference
1.02 / 01-2017




                 R-72             A+W Production Formula Editor
Formula Editor                R

                        Partindex




                 A+W Production
                 Partindex                                                 Index Formula Editor




                 Index Formula Editor
                 A                                – Level I R-11
                 AddUp                            – Level II R-16
                 – Quantity Editor R-61           – Normal R-52
                 Airspace                         – Top input field R-51
                 – Enter Value (Numeric) R-56     – Value R-52
                 All                              Condition Name
                 – Conditions - Editor R-50       – Dialog R-53
                 – Quantity Editor R-61           – New Name R-53
                 Allocation                       – Old Name R-53
                 – Level I R-15                   Conditions
                 – Level II R-18                  – Condition R-52
                 Allocation Editor                Conditions - Author
                 – Characteristic R-70            – Menu R-49
                 – Dialog R-69                    – Tool bar R-49
                 – Formula R-71                   Conditions - Editor
                 – Given Quantity R-71            – All R-50
                 – Quantity R-71                  – Dialog R-48
                 – Top input field R-70           – Null R-50
                 And Operation                    – One R-50
                 – Formula Editor R-67
                 Anychild                         D
                 – Quantity Editor R-61           Delete
                 Average                          – Select Allocation R-69
                 – Formula Editor R-67            – Select Conditions R-47
                                                  – Select Formula R-65
                 B                                – Select Quantity R-58
                 Bottom                           Description
                 – Quantity Editor R-61           – Formula Editor R-67
                 Bottom input field               – Select Allocation R-69
                 – Condition R-52                 – Select Conditions R-47
                                                  – Select Formula R-65
                                                  – Select Quantity R-58
                 C
                                                  Dialog
                 Central selection field
                                                  – Allocation Editor R-69
                 – Condition R-52
                                                  – Condition Name R-53
                 Characteristic
                                                  – Conditions-Editor R-48
                 – Allocation Editor R-70
                                                  – Enter Value (Numeric) R-55
                 Child
                                                  – Formula Editor R-66
                 – Quantity Editor R-61
                                                  – Info R-54, R-63
                 Comparison
                                                  – Quantity Editor R-59
                 – Level I R-11
                                                  – Quantity Name R-61
                 – Level II R-16
                                                  – Select Allocation R-69
                 Condition
                                                  – Select Conditions R-46
                 – Bottom input field R-52
                                                  – Select Formulas R-64
                 – Central selection field R-52
                                                  – Select Quantity R-57
                 – Condition R-51
                                                  Digit
1.02 / 01-2017




                 – Conditions R-52
                                                  – Enter Value (Numeric) R-56
                 – Given Quantity R-55
                 – Invert R-54


                 A+W Production Formula Editor                                           R-75
                 Index Formula Editor                                              Partindex




                 E                             G
                 Edit                          Given Quantity
                 – Select Allocation R-69      – Allocation Editor R-71
                 – Select Conditions R-47      – Condition R-55
                 – Select Formula R-65
                 – Select quantity R-58        I
                 Enter Value (Numeric)         Info
                 – Airspace R-56               – Dialog R-54, R-63
                 – Dialog R-55                 Invert
                 – Digit R-56                  – Condition R-54
                 – Length R-56
                 – New Value R-56
                 – Old Value R-56              L
                 – Text R-56                   Length
                 – Thickness R-56              – Enter Value (Numeric) R-56
                 Existing Allocation
                 – Select Allocation R-69      M
                 Existing Conditions           Master
                 – Select Conditions R-46      – Quantity creator R-61
                 Existing Formulas             Maximum
                 – Formula Editor R-68         – Formula Editor R-67
                 – Select Formula R-65         Menu
                 Existing Properties           – Conditions-Author R-49
                 – Formula Editor R-68         – Quantity creator R-60
                 Existing Quantity             Minimum
                 – Select Quantity R-58        – Formula Editor R-67

                 F                             N
                 Formula                       New Allocation
                 – Allocation Editor R-71      – Select Allocation R-69
                 – Formula Editor R-67         New Condition
                 – Level I R-10                – Select Conditions R-47
                 – Level II R-15               New Formula
                 Formula Editor                – Select Formula R-65
                 – And Operation R-67          New Name
                 – Average R-67                – Condition Name R-53
                 – Description R-67            – Quantity Name R-62
                 – Dialog R-66                 New Quantity
                 – Existing Formulas R-68      – Select Quantity R-58
                 – Existing Properties R-68    New Value
                 – Formula R-67                – Enter Value (Numeric) R-56
                 – Maximum R-67                No Allocation
                 – Minimum R-67                – Select Allocation R-69
                 – Number of Results R-67      No Condition
                 – Or Operation R-67           – Select Conditions R-47
                 – Quantity R-67               No Formula
                 – Top input field R-67        – Select Formula R-65
                 – Total R-67                  No Quantity
                 Formula editor                – Select Quantity R-58
1.02 / 01-2017




                 – Transferred quantity R-67   Normal
                                               – Condition R-52




                 R-76                                          A+W Production Formula Editor
                 Partindex                                                     Index Formula Editor




                 Null                            – Edit R-69
                 – Condition - Editor R-50       – Existing Allocations R-69
                 Number of Results               – New Allocation R-69
                 – Formula Editor R-67           – No Allocation R-69
                                                 Select Conditions
                 O                               – Delete R-47
                 Old Name                        – Description R-47
                 – Condition Name R-53           – Dialog R-46
                 – Quantity Name R-62            – Edit R-47
                 Old Value                       – Existing Conditions R-46
                 – Enter Value (Numeric) R-56    – New Condition R-47
                 One                             – No Condition R-47
                 – Conditions - Editor R-50      Select Formula
                 Or Operation                    – Delete R-65
                 – Formula Editor R-67           – Description R-65
                                                 – Edit R-65
                                                 – Existing Formulas R-65
                 P                               – New Formula R-65
                 Parent                          – No Formula R-65
                 – Quantity Editor   R-61        Select Formulas
                                                 – Dialog R-64
                 Q                               Select Quantity
                 Quantity                        – Delete R-58
                 – Allocation Editor R-71        – Description R-58
                 – Formula Editor R-67           – Dialog R-57
                 – Level I R-14                  – Existing Quantity R-58
                 – Level II R-17                 – New Quantity R-58
                 – Level III R-18                – No Quantity R-58
                 Quantity creator                Select quantity
                 – Master R-61                   – Edit R-58
                 – Menu R-60                     Self
                 Quantity Editor                 – Quantity Editor R-61
                 – AddUp R-61
                 – All R-61                      T
                 – Anychild R-61                 Text
                 – Bottom R-61                   – Enter Value (Numeric) R-56
                 – Child R-61                    Thickness Value
                 – Dialog R-59                   – Enter Value (Numeric) R-56
                 – Parent R-61                   Tool bar
                 – Self R-61                     – Conditions-Author R-49
                 – Tool bar R-60                 – Quantity Editor R-60
                 – Up R-61                       Top input field
                 Quantity Name                   – Allocation Editor R-70
                 – Dialog R-61                   – Condition R-51
                 – New Name R-62                 – Formula Editor R-67
                 – Old Name R-62                 Total
                                                 – Formula Editor R-67
                 S                               Transferred quantity
                 Select Allocation               – Formula editor R-67
1.02 / 01-2017




                 – Delete R-69
                 – Description R-69
                 – Dialog R-69



                 A+W Production Formula Editor                                               R-77
                 Index Formula Editor                            Partindex




                 U
                 Up
                 – Quantity Editor    R-61

                 V
                 Value
                 – Condition   R-52
1.02 / 01-2017




                 R-78                        A+W Production Formula Editor

