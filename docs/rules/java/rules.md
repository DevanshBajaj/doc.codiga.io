---
id: rules-java
title: Java rules
description: Code Analysis rules of Codiga for Java detecting good software practices, security and vulnerability issues. Available on GitHub, GitLab and Bitbucket.
keywords:
  - cyclomatic complexity
  - function complexity
  - function length
  - code quality
  - software quality
  - codiga
  - static analysis
  - static code analysis
  - continuous integration
  - ci/cd pipeline
  - code verification
  - security analysis
  - CWE
  - CVE
  - Java
---

| Rule                                                                                                                                                               | Category       | Severity | Description                                                                                                                                   |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------- | -------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| [AbstractClassWithoutAbstractMethod](https://pmd.github.io/pmd/pmd_rules_java_bestpractices.html#abstractclasswithoutabstractmethod)                               | Best Practices | 3        | This abstract class does not have any abstract methods                                                                                        |
| [AbstractClassWithoutAnyMethod](https://pmd.github.io/pmd/pmd_rules_java_design.html#abstractclasswithoutanymethod)                                                | Design         | 1        | No abstract method which means that the keyword is most likely used to prevent instantiation. Use a private or protected constructor instead. |
| [AssignmentToNonFinalStatic](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#assignmenttononfinalstatic)                                                  | Error Prone    | 3        | Possible unsafe assignment to a non-final static field in a constructor.                                                                      |
| [AvoidBranchingStatementAsLastInLoop](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#avoidbranchingstatementaslastinloop)                                | Error Prone    | 2        | Avoid using a branching statement as the last in a loop.                                                                                      |
| [AvoidDecimalLiteralsInBigDecimalConstructor](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#avoiddecimalliteralsinbigdecimalconstructor)                | Error Prone    | 3        | Avoid creating BigDecimal with a decimal (float/double) literal. Use a String literal                                                         |
| [AvoidDeeplyNestedIfStmts](https://pmd.github.io/pmd/pmd_rules_java_design.html#avoiddeeplynestedifstmts)                                                          | Design         | 3        | Deeply nested if..then statements are hard to read                                                                                            |
| [AvoidInstanceofChecksInCatchClause](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#avoidinstanceofchecksincatchclause)                                  | Error Prone    | 3        | An instanceof check is being performed on the caught exception. Create a separate catch clause for this exception type.                       |
| [AvoidMultipleUnaryOperators](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#avoidmultipleunaryoperators)                                                | Error Prone    | 2        | Using multiple unary operators may be a bug                                                                                                   |
| [AvoidProtectedFieldInFinalClass](https://pmd.github.io/pmd/pmd_rules_java_codestyle.html#avoidprotectedfieldinfinalclass)                                         | Code Style     | 3        | Avoid protected fields in a final class. Change to private or package access.                                                                 |
| [AvoidProtectedMethodInFinalClassNotExtending](https://pmd.github.io/pmd/pmd_rules_java_codestyle.html#avoidprotectedmethodinfinalclassnotextending)               | Code Style     | 3        | Avoid protected methods in a final class that doesnt extend anything other than Object. Change to private or package access.                  |
| [AvoidReassigningParameters](https://pmd.github.io/pmd/pmd_rules_java_bestpractices.html#avoidreassigningparameters)                                               | Best Practices | 2        | Avoid reassigning parameters                                                                                                                  |
| [AvoidSynchronizedAtMethodLevel](https://pmd.github.io/pmd/pmd_rules_java_multithreading.html#avoidsynchronizedatmethodlevel)                                      | Unknonwn       | 3        | Use block level rather than method level synchronization                                                                                      |
| [AvoidThreadGroup](https://pmd.github.io/pmd/pmd_rules_java_multithreading.html#avoidthreadgroup)                                                                  | Unknonwn       | 3        | Avoid using java.lang.ThreadGroup; it is not thread safe                                                                                      |
| [AvoidUsingHardCodedIP](https://pmd.github.io/pmd/pmd_rules_java_bestpractices.html#avoidusinghardcodedip)                                                         | Best Practices | 3        | Do not hard code the IP address                                                                                                               |
| [AvoidUsingOctalValues](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#avoidusingoctalvalues)                                                            | Error Prone    | 3        | Do not start a literal by 0 unless its an octal value                                                                                         |
| [BadComparison](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#badcomparison)                                                                            | Error Prone    | 3        | Avoid equality comparisons with Double.NaN                                                                                                    |
| [BigIntegerInstantiation](https://pmd.github.io/pmd/pmd_rules_java_performance.html#bigintegerinstantiation)                                                       | Unknonwn       | 3        | Dont create instances of already existing BigInteger and BigDecimal.                                                                          |
| [BooleanInstantiation](https://pmd.github.io/pmd/pmd_rules_java_performance.html#booleaninstantiation)                                                             | Unknonwn       | 2        | Avoid instantiating Boolean objects; reference Boolean.TRUE or Boolean.FALSE or call Boolean.valueOf() instead.                               |
| [BrokenNullCheck](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#brokennullcheck)                                                                        | Error Prone    | 2        | Method call on object which may be null                                                                                                       |
| [CheckResultSet](https://pmd.github.io/pmd/pmd_rules_java_bestpractices.html#checkresultset)                                                                       | Best Practices | 3        | Always check the return of one of the navigation method (next                                                                                 |
| [CheckSkipResult](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#checkskipresult)                                                                        | Error Prone    | 3        | Check the value returned by the skip() method of an InputStream to see if the requested number of bytes has been skipped.                     |
| [ClassCastExceptionWithToArray](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#classcastexceptionwithtoarray)                                            | Error Prone    | 3        | This usage of the Collection.toArray() method will throw a ClassCastException.                                                                |
| [ClassWithOnlyPrivateConstructorsShouldBeFinal](https://pmd.github.io/pmd/pmd_rules_java_design.html#classwithonlyprivateconstructorsshouldbefinal)                | Design         | 1        | A class which only has private constructors should be final                                                                                   |
| [CloseResource](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#closeresource)                                                                            | Error Prone    | 3        | Ensure that resources like this PipedWriter object are closed after use                                                                       |
| [CollapsibleIfStatements](https://pmd.github.io/pmd/pmd_rules_java_design.html#collapsibleifstatements)                                                            | Design         | 3        | These nested if statements could be combined                                                                                                  |
| [CompareObjectsWithEquals](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#compareobjectswithequals)                                                      | Error Prone    | 3        | Use equals() to compare object references.                                                                                                    |
| [ConfusingTernary](https://pmd.github.io/pmd/pmd_rules_java_codestyle.html#confusingternary)                                                                       | Code Style     | 3        | Avoid if (x != y) ..; else ..;                                                                                                                |
| [ConstantsInInterface](https://pmd.github.io/pmd/pmd_rules_java_bestpractices.html#constantsininterface)                                                           | Best Practices | 3        | Avoid constants in interfaces. Interfaces define types                                                                                        |
| [ConstructorCallsOverridableMethod](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#constructorcallsoverridablemethod)                                    | Error Prone    | 1        | Overridable method 'getAction' called during object construction                                                                              |
| [DataClass](https://pmd.github.io/pmd/pmd_rules_java_design.html#dataclass)                                                                                        | Design         | 3        | The class is suspected to be a Data Class                                                                                                     |
| [DefaultLabelNotLastInSwitchStmt](https://pmd.github.io/pmd/pmd_rules_java_bestpractices.html#defaultlabelnotlastinswitchstmt)                                     | Best Practices | 3        | The default label should be the last label in a switch statement                                                                              |
| [DontCallThreadRun](https://pmd.github.io/pmd/pmd_rules_java_multithreading.html#dontcallthreadrun)                                                                | Unknonwn       | 4        | Dont call Thread.run() explicitly                                                                                                             |
| [DontUseFloatTypeForLoopIndices](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#dontusefloattypeforloopindices)                                          | Error Prone    | 3        | Dont use floating point for loop indices. If you must use floating point                                                                      |
| [DoubleCheckedLocking](https://pmd.github.io/pmd/pmd_rules_java_multithreading.html#doublecheckedlocking)                                                          | Unknonwn       | 1        | Double checked locking is not thread safe in Java.                                                                                            |
| [EmptyMethodInAbstractClassShouldBeAbstract](https://pmd.github.io/pmd/pmd_rules_java_codestyle.html#emptymethodinabstractclassshouldbeabstract)                   | Code Style     | 1        | An empty method in an abstract class should be abstract instead                                                                               |
| [EqualsNull](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#equalsnull)                                                                                  | Error Prone    | 1        | Avoid using equals() to compare against null                                                                                                  |
| [ExtendsObject](https://pmd.github.io/pmd/pmd_rules_java_codestyle.html#extendsobject)                                                                             | Code Style     | 4        | No need to explicitly extend Object.                                                                                                          |
| [FieldDeclarationsShouldBeAtStartOfClass](https://pmd.github.io/pmd/pmd_rules_java_codestyle.html#fielddeclarationsshouldbeatstartofclass)                         | Code Style     | 3        | Fields should be declared at the top of the class                                                                                             |
| [FinalFieldCouldBeStatic](https://pmd.github.io/pmd/pmd_rules_java_design.html#finalfieldcouldbestatic)                                                            | Design         | 3        | This final field could be made static                                                                                                         |
| [ForLoopShouldBeWhileLoop](https://pmd.github.io/pmd/pmd_rules_java_codestyle.html#forloopshouldbewhileloop)                                                       | Code Style     | 3        | This for loop could be simplified to a while loop                                                                                             |
| [GodClass](https://pmd.github.io/pmd/pmd_rules_java_design.html#godclass)                                                                                          | Design         | 3        | Possible God Class                                                                                                                            |
| [IdempotentOperations](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#idempotentoperations)                                                              | Error Prone    | 3        | Avoid idempotent operations (like assigning a variable to itself).                                                                            |
| [ImmutableField](https://pmd.github.io/pmd/pmd_rules_java_design.html#immutablefield)                                                                              | Design         | 3        | Private field could be made final; it is only initialized in the declaration or constructor.                                                  |
| [InstantiationToGetClass](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#instantiationtogetclass)                                                        | Error Prone    | 4        | Avoid instantiating an object just to call getClass() on it; use the .class public member instead                                             |
| [JumbledIncrementer](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#jumbledincrementer)                                                                  | Error Prone    | 3        | Avoid modifying an outer loop incrementer in an inner loop for update expression                                                              |
| [LogicInversion](https://pmd.github.io/pmd/pmd_rules_java_design.html#logicinversion)                                                                              | Design         | 3        | Use opposite operator instead of the logic complement operator.                                                                               |
| [MisplacedNullCheck](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#misplacednullcheck)                                                                  | Error Prone    | 3        | The null check here is misplaced; if the variable is null there will be a NullPointerException                                                |
| [MissingBreakInSwitch](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#missingbreakinswitch)                                                              | Error Prone    | 3        | A switch statement does not contain a break                                                                                                   |
| [MissingStaticMethodInNonInstantiatableClass](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#missingstaticmethodinnoninstantiatableclass)                | Error Prone    | 3        | Class cannot be instantiated and does not provide any static methods or fields                                                                |
| [NonCaseLabelInSwitchStatement](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#noncaselabelinswitchstatement)                                            | Error Prone    | 3        | A non-case label was present in a switch statement                                                                                            |
| [NonStaticInitializer](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#nonstaticinitializer)                                                              | Error Prone    | 3        | Non-static initializers are confusing                                                                                                         |
| [NonThreadSafeSingleton](https://pmd.github.io/pmd/pmd_rules_java_multithreading.html#nonthreadsafesingleton)                                                      | Unknonwn       | 3        | Singleton is not thread safe                                                                                                                  |
| [OptimizableToArrayCall](https://pmd.github.io/pmd/pmd_rules_java_performance.html#optimizabletoarraycall)                                                         | Unknonwn       | 3        | This call to Collection.toArray() may be optimizable                                                                                          |
| [OverrideBothEqualsAndHashcode](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#overridebothequalsandhashcode)                                            | Error Prone    | 3        | Ensure you override both equals() and hashCode()                                                                                              |
| [PositionLiteralsFirstInCaseInsensitiveComparisons](https://pmd.github.io/pmd/pmd_rules_java_bestpractices.html#positionliteralsfirstincaseinsensitivecomparisons) | Best Practices | 3        | Position literals first in String comparisons for EqualsIgnoreCase                                                                            |
| [PositionLiteralsFirstInComparisons](https://pmd.github.io/pmd/pmd_rules_java_bestpractices.html#positionliteralsfirstincomparisons)                               | Best Practices | 3        | Position literals first in String comparisons                                                                                                 |
| [PreserveStackTrace](https://pmd.github.io/pmd/pmd_rules_java_bestpractices.html#preservestacktrace)                                                               | Best Practices | 3        | New exception is thrown in catch block                                                                                                        |
| [ReturnEmptyArrayRatherThanNull](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#returnemptyarrayratherthannull)                                          | Error Prone    | 1        | Return an empty array rather than null.                                                                                                       |
| [ReturnFromFinallyBlock](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#returnfromfinallyblock)                                                          | Error Prone    | 3        | Avoid returning from a finally block                                                                                                          |
| [SimpleDateFormatNeedsLocale](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#simpledateformatneedslocale)                                                | Error Prone    | 3        | When instantiating a SimpleDateFormat object                                                                                                  |
| [SimplifiedTernary](https://pmd.github.io/pmd/pmd_rules_java_design.html#simplifiedternary)                                                                        | Design         | 3        | Ternary operators that can be simplified                                                                                                      |
| [SimplifyBooleanExpressions](https://pmd.github.io/pmd/pmd_rules_java_design.html#simplifybooleanexpressions)                                                      | Design         | 3        | Avoid unnecessary comparisons in boolean expressions                                                                                          |
| [SimplifyBooleanReturns](https://pmd.github.io/pmd/pmd_rules_java_design.html#simplifybooleanreturns)                                                              | Design         | 3        | Avoid unnecessary if..then..else statements when returning booleans                                                                           |
| [SimplifyConditional](https://pmd.github.io/pmd/pmd_rules_java_design.html#simplifyconditional)                                                                    | Design         | 3        | No need to check for null before an instanceof                                                                                                |
| [SingleMethodSingleton](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#singlemethodsingleton)                                                            | Error Prone    | 2        | Class contains multiple getInstance methods. Please review.                                                                                   |
| [SingletonClassReturningNewInstance](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#singletonclassreturningnewinstance)                                  | Error Prone    | 2        | getInstance method always creates a new object and hence does not comply to Singleton Design Pattern behaviour. Please review                 |
| [SingularField](https://pmd.github.io/pmd/pmd_rules_java_design.html#singularfield)                                                                                | Design         | 3        | Replace with a local variable.                                                                                                                |
| [SwitchDensity](https://pmd.github.io/pmd/pmd_rules_java_design.html#switchdensity)                                                                                | Design         | 3        | A high ratio of statements to labels in a switch statement. Consider refactoring.                                                             |
| [SwitchStmtsShouldHaveDefault](https://pmd.github.io/pmd/pmd_rules_java_bestpractices.html#switchstmtsshouldhavedefault)                                           | Best Practices | 3        | Switch statements should have a default label                                                                                                 |
| [TooFewBranchesForASwitchStatement](https://pmd.github.io/pmd/pmd_rules_java_performance.html#toofewbranchesforaswitchstatement)                                   | Unknonwn       | 3        | A switch with less than three branches is inefficient                                                                                         |
| [UncommentedEmptyConstructor](https://pmd.github.io/pmd/pmd_rules_java_documentation.html#uncommentedemptyconstructor)                                             | Documentation  | 3        | Document empty constructor                                                                                                                    |
| [UncommentedEmptyMethodBody](https://pmd.github.io/pmd/pmd_rules_java_documentation.html#uncommentedemptymethodbody)                                               | Documentation  | 3        | Document empty method body                                                                                                                    |
| [UnconditionalIfStatement](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#unconditionalifstatement)                                                      | Error Prone    | 3        | Do not use if statements that are always true or always false                                                                                 |
| [UnnecessaryLocalBeforeReturn](https://pmd.github.io/pmd/pmd_rules_java_codestyle.html#unnecessarylocalbeforereturn)                                               | Code Style     | 3        | Consider simply returning the value vs storing it in local variable 'searchOptions'                                                           |
| [UnsynchronizedStaticDateFormatter](https://pmd.github.io/pmd/pmd_rules_java_multithreading.html#unsynchronizedstaticdateformatter)                                | Unknonwn       | 3        | Static DateFormatter objects should be accessed in a synchronized manner                                                                      |
| [UseCollectionIsEmpty](https://pmd.github.io/pmd/pmd_rules_java_bestpractices.html#usecollectionisempty)                                                           | Best Practices | 3        | Substitute calls and make them more efficient                                                                                                 |
| [UseLocaleWithCaseConversions](https://pmd.github.io/pmd/pmd_rules_java_errorprone.html#uselocalewithcaseconversions)                                              | Error Prone    | 3        | Use explicit locale when doing a String.toLowerCase()/toUpperCase() call                                                                      |
| [UseNotifyAllInsteadOfNotify](https://pmd.github.io/pmd/pmd_rules_java_multithreading.html#usenotifyallinsteadofnotify)                                            | Unknonwn       | 3        | Call Thread.notifyAll() rather than Thread.notify()                                                                                           |
| [UseUtilityClass](https://pmd.github.io/pmd/pmd_rules_java_design.html#useutilityclass)                                                                            | Design         | 3        | All methods are static. Consider using a utility class instead. Alternatively                                                                 |
| [UseVarargs](https://pmd.github.io/pmd/pmd_rules_java_bestpractices.html#usevarargs)                                                                               | Best Practices | 4        | Consider using varargs for methods or constructors which take an array the last parameter.                                                    |