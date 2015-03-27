
vendor/bin/phpcs tests/* --standard=phpcs.xml --extensions=php -s --report=source

PHP CODE SNIFFER VIOLATION SOURCE SUMMARY
----------------------------------------------------------------------
SOURCE                                                           COUNT
----------------------------------------------------------------------
Generic.CodeAnalysis.UnusedFunctionParameter.Found               20
Generic.Files.LineLength.MaxExceeded                             6
PSR1.Classes.ClassDeclaration.MultipleClasses                    3
Generic.Files.OneClassPerFile.MultipleFound                      3
Generic.Metrics.NestingLevel.MaxExceeded                         3
PSR1.Files.SideEffects.FoundWithSymbols                          3
Generic.PHP.SAPIUsage.FunctionFound                              2
Generic.CodeAnalysis.EmptyStatement.DetectedFOREACH              1
Generic.CodeAnalysis.UselessOverridingMethod.Found               1
Generic.CodeAnalysis.EmptyStatement.DetectedCATCH                1
Generic.Metrics.CyclomaticComplexity.MaxExceeded                 1
Squiz.Scope.MethodScope.Missing                                  1
Internal.NoCodeFound                                             1
----------------------------------------------------------------------
A TOTAL OF 46 SNIFF VIOLATIONS WERE FOUND IN 13 SOURCES
----------------------------------------------------------------------

############################################################################

vendor/bin/phpcs tests/* --standard=phpcs.xml --extensions=php -sp

EE.....W......E......................................E.....W  60 / 419 (14%)
..W..........................W..W.........W......W.......... 120 / 419 (29%)
................E...........E....E.................EW..E..W. 180 / 419 (43%)
...W....................E......W......W.W.............W..... 240 / 419 (57%)
.............................E.............W................ 300 / 419 (72%)
...........E........W............W.......................... 360 / 419 (86%)
.......................................E..........W......EW


FILE: ...ww/html/mediawiki-1.24.1/extensions/SemanticMediaWiki/tests/autoloader.php
--------------------------------------------------------------------------------
FOUND 1 ERROR AFFECTING 1 LINE
--------------------------------------------------------------------------------
 12 | ERROR | Use the PHP_SAPI constant instead of calling php_sapi_name()
    |       | (Generic.PHP.SAPIUsage.FunctionFound)
--------------------------------------------------------------------------------


FILE: ...www/html/mediawiki-1.24.1/extensions/SemanticMediaWiki/tests/bootstrap.php
--------------------------------------------------------------------------------
FOUND 2 ERRORS AFFECTING 2 LINES
--------------------------------------------------------------------------------
 3 | ERROR | Use the PHP_SAPI constant instead of calling php_sapi_name()
   |       | (Generic.PHP.SAPIUsage.FunctionFound)
 9 | ERROR | Line exceeds maximum limit of 180 characters; contains 228
   |       | characters (Generic.Files.LineLength.MaxExceeded)
--------------------------------------------------------------------------------


FILE: ...1/extensions/SemanticMediaWiki/tests/phpunit/Utils/Mock/FakeQueryStore.php
--------------------------------------------------------------------------------
FOUND 0 ERRORS AND 1 WARNING AFFECTING 1 LINE
--------------------------------------------------------------------------------
 32 | WARNING | The method parameter $query is never used
    |         | (Generic.CodeAnalysis.UnusedFunctionParameter.Found)
--------------------------------------------------------------------------------


FILE: .../extensions/SemanticMediaWiki/tests/phpunit/Utils/File/LocalFileUpload.php
--------------------------------------------------------------------------------
FOUND 1 ERROR AFFECTING 1 LINE
--------------------------------------------------------------------------------
 99 | ERROR | Visibility must be declared on method "initializeFromRequest"
    |       | (Squiz.Scope.MethodScope.Missing)
--------------------------------------------------------------------------------


FILE: .../SemanticMediaWiki/tests/phpunit/Utils/Validators/QueryResultValidator.php
--------------------------------------------------------------------------------
FOUND 2 ERRORS AFFECTING 2 LINES
--------------------------------------------------------------------------------
 51 | ERROR | Function's nesting level (5) exceeds allowed maximum of 3
    |       | (Generic.Metrics.NestingLevel.MaxExceeded)
 94 | ERROR | Function's nesting level (5) exceeds allowed maximum of 3
    |       | (Generic.Metrics.NestingLevel.MaxExceeded)
--------------------------------------------------------------------------------


FILE: ...ki-1.24.1/extensions/SemanticMediaWiki/tests/phpunit/Utils/PageCreator.php
--------------------------------------------------------------------------------
FOUND 0 ERRORS AND 1 WARNING AFFECTING 1 LINE
--------------------------------------------------------------------------------
 1 | WARNING | A file should declare new symbols (classes, functions, constants,
   |         | etc.) and cause no other side effects, or it should execute logic with
   |         | side effects, but should not do both. The first symbol is defined on
   |         | line 16 and the first side effect is on line 101.
   |         | (PSR1.Files.SideEffects.FoundWithSymbols)
--------------------------------------------------------------------------------


FILE: ...nsions/SemanticMediaWiki/tests/phpunit/Utils/Runners/MaintenanceRunner.php
--------------------------------------------------------------------------------
FOUND 0 ERRORS AND 1 WARNING AFFECTING 1 LINE
--------------------------------------------------------------------------------
 1 | WARNING | A file should declare new symbols (classes, functions, constants,
   |         | etc.) and cause no other side effects, or it should execute logic with
   |         | side effects, but should not do both. The first symbol is defined on
   |         | line 22 and the first side effect is on line 105.
   |         | (PSR1.Files.SideEffects.FoundWithSymbols)
--------------------------------------------------------------------------------


FILE: ...SemanticMediaWiki/tests/phpunit/includes/Maintenance/DataRebuilderTest.php
--------------------------------------------------------------------------------
FOUND 0 ERRORS AND 3 WARNINGS AFFECTING 1 LINE
--------------------------------------------------------------------------------
 321 | WARNING | The method parameter $count is never used
     |         | (Generic.CodeAnalysis.UnusedFunctionParameter.Found)
 321 | WARNING | The method parameter $namespaces is never used
     |         | (Generic.CodeAnalysis.UnusedFunctionParameter.Found)
 321 | WARNING | The method parameter $usejobs is never used
     |         | (Generic.CodeAnalysis.UnusedFunctionParameter.Found)
--------------------------------------------------------------------------------


FILE: ...diaWiki/tests/phpunit/includes/Annotator/RedirectPropertyAnnotatorTest.php
--------------------------------------------------------------------------------
FOUND 0 ERRORS AND 1 WARNING AFFECTING 1 LINE
--------------------------------------------------------------------------------
 34 | WARNING | Possible useless method overriding detected
    |         | (Generic.CodeAnalysis.UselessOverridingMethod.Found)
--------------------------------------------------------------------------------


FILE: ...nticMediaWiki/tests/phpunit/includes/parserhooks/SetParserFunctionTest.php
--------------------------------------------------------------------------------
FOUND 0 ERRORS AND 1 WARNING AFFECTING 1 LINE
--------------------------------------------------------------------------------
 67 | WARNING | The method parameter $expected is never used
    |         | (Generic.CodeAnalysis.UnusedFunctionParameter.Found)
--------------------------------------------------------------------------------


FILE: ...nticMediaWiki/tests/phpunit/includes/parserhooks/AskParserFunctionTest.php
--------------------------------------------------------------------------------
FOUND 0 ERRORS AND 1 WARNING AFFECTING 1 LINE
--------------------------------------------------------------------------------
 75 | WARNING | The method parameter $expected is never used
    |         | (Generic.CodeAnalysis.UnusedFunctionParameter.Found)
--------------------------------------------------------------------------------


FILE: ...Wiki/tests/phpunit/includes/SPARQLStore/SparqlDBConnectionProviderTest.php
--------------------------------------------------------------------------------
FOUND 2 ERRORS AFFECTING 1 LINE
--------------------------------------------------------------------------------
 223 | ERROR | Only one class is allowed in a file
     |       | (Generic.Files.OneClassPerFile.MultipleFound)
 223 | ERROR | Each class must be in a file by itself
     |       | (PSR1.Classes.ClassDeclaration.MultipleClasses)
--------------------------------------------------------------------------------


FILE: ...nsions/SemanticMediaWiki/tests/phpunit/includes/dataitems/DataItemTest.php
--------------------------------------------------------------------------------
FOUND 1 ERROR AFFECTING 1 LINE
--------------------------------------------------------------------------------
 53 | ERROR | Empty FOREACH statement detected
    |       | (Generic.CodeAnalysis.EmptyStatement.DetectedFOREACH)
--------------------------------------------------------------------------------


FILE: ...ensions/SemanticMediaWiki/tests/phpunit/includes/specials/SpecialsTest.php
--------------------------------------------------------------------------------
FOUND 1 ERROR AFFECTING 1 LINE
--------------------------------------------------------------------------------
 79 | ERROR | Function's nesting level (4) exceeds allowed maximum of 3
    |       | (Generic.Metrics.NestingLevel.MaxExceeded)
--------------------------------------------------------------------------------


FILE: ...tensions/SemanticMediaWiki/tests/phpunit/includes/DataTypeRegistryTest.php
--------------------------------------------------------------------------------
FOUND 2 ERRORS AFFECTING 1 LINE
--------------------------------------------------------------------------------
 201 | ERROR | Only one class is allowed in a file
     |       | (Generic.Files.OneClassPerFile.MultipleFound)
 201 | ERROR | Each class must be in a file by itself
     |       | (PSR1.Classes.ClassDeclaration.MultipleClasses)
--------------------------------------------------------------------------------


FILE: ...ns/SemanticMediaWiki/tests/phpunit/includes/PropertyTypeDiffFinderTest.php
--------------------------------------------------------------------------------
FOUND 0 ERRORS AND 2 WARNINGS AFFECTING 1 LINE
--------------------------------------------------------------------------------
 167 | WARNING | The method parameter $subject is never used
     |         | (Generic.CodeAnalysis.UnusedFunctionParameter.Found)
 167 | WARNING | The method parameter $requestoptions is never used
     |         | (Generic.CodeAnalysis.UnusedFunctionParameter.Found)
--------------------------------------------------------------------------------


FILE: ...sions/SemanticMediaWiki/tests/phpunit/includes/DataValues/UriValueTest.php
--------------------------------------------------------------------------------
FOUND 3 ERRORS AFFECTING 3 LINES
--------------------------------------------------------------------------------
 320 | ERROR | Line exceeds maximum limit of 180 characters; contains 190
     |       | characters (Generic.Files.LineLength.MaxExceeded)
 322 | ERROR | Line exceeds maximum limit of 180 characters; contains 190
     |       | characters (Generic.Files.LineLength.MaxExceeded)
 333 | ERROR | Line exceeds maximum limit of 180 characters; contains 190
     |       | characters (Generic.Files.LineLength.MaxExceeded)
--------------------------------------------------------------------------------


FILE: ...4.1/extensions/SemanticMediaWiki/tests/phpunit/includes/UrlEncoderTest.php
--------------------------------------------------------------------------------
FOUND 0 ERRORS AND 1 WARNING AFFECTING 1 LINE
--------------------------------------------------------------------------------
 42 | WARNING | The method parameter $input is never used
    |         | (Generic.CodeAnalysis.UnusedFunctionParameter.Found)
--------------------------------------------------------------------------------


FILE: ...24.1/extensions/SemanticMediaWiki/tests/phpunit/includes/SubobjectTest.php
--------------------------------------------------------------------------------
FOUND 0 ERRORS AND 1 WARNING AFFECTING 1 LINE
--------------------------------------------------------------------------------
 209 | WARNING | The method parameter $expected is never used
     |         | (Generic.CodeAnalysis.UnusedFunctionParameter.Found)
--------------------------------------------------------------------------------


FILE: ...manticMediaWiki/tests/phpunit/includes/dic/SimpleDependencyBuilderTest.php
--------------------------------------------------------------------------------
FOUND 2 ERRORS AFFECTING 1 LINE
--------------------------------------------------------------------------------
 859 | ERROR | Only one class is allowed in a file
     |       | (Generic.Files.OneClassPerFile.MultipleFound)
 859 | ERROR | Each class must be in a file by itself
     |       | (PSR1.Classes.ClassDeclaration.MultipleClasses)
--------------------------------------------------------------------------------


FILE: ...diaWiki/tests/phpunit/includes/formatters/ParserParameterFormatterTest.php
--------------------------------------------------------------------------------
FOUND 0 ERRORS AND 1 WARNING AFFECTING 1 LINE
--------------------------------------------------------------------------------
 108 | WARNING | The method parameter $params is never used
     |         | (Generic.CodeAnalysis.UnusedFunctionParameter.Found)
--------------------------------------------------------------------------------


FILE: ...ediaWiki/tests/phpunit/includes/MediaWiki/Jobs/UpdateDispatcherJobTest.php
--------------------------------------------------------------------------------
FOUND 0 ERRORS AND 1 WARNING AFFECTING 1 LINE
--------------------------------------------------------------------------------
 299 | WARNING | The method parameter $requestoptions is never used
     |         | (Generic.CodeAnalysis.UnusedFunctionParameter.Found)
--------------------------------------------------------------------------------


FILE: ...SemanticMediaWiki/tests/phpunit/includes/MediaWiki/Jobs/RefreshJobTest.php
--------------------------------------------------------------------------------
FOUND 0 ERRORS AND 2 WARNINGS AFFECTING 1 LINE
--------------------------------------------------------------------------------
 177 | WARNING | The method parameter $count is never used
     |         | (Generic.CodeAnalysis.UnusedFunctionParameter.Found)
 177 | WARNING | The method parameter $namespaces is never used
     |         | (Generic.CodeAnalysis.UnusedFunctionParameter.Found)
--------------------------------------------------------------------------------


FILE: ...ticMediaWiki/tests/phpunit/includes/MediaWiki/RedirectTargetFinderTest.php
--------------------------------------------------------------------------------
FOUND 0 ERRORS AND 2 WARNINGS AFFECTING 1 LINE
--------------------------------------------------------------------------------
 53 | WARNING | The method parameter $expectedHasTarget is never used
    |         | (Generic.CodeAnalysis.UnusedFunctionParameter.Found)
 53 | WARNING | The method parameter $expectedGetTarget is never used
    |         | (Generic.CodeAnalysis.UnusedFunctionParameter.Found)
--------------------------------------------------------------------------------


FILE: ...emanticMediaWiki/tests/phpunit/includes/MediaWiki/HtmlTableBuilderTest.php
--------------------------------------------------------------------------------
FOUND 1 ERROR AFFECTING 1 LINE
--------------------------------------------------------------------------------
 162 | ERROR | Line exceeds maximum limit of 180 characters; contains 186
     |       | characters (Generic.Files.LineLength.MaxExceeded)
--------------------------------------------------------------------------------


FILE: ...SemanticMediaWiki/tests/phpunit/includes/Factbox/FactboxMagicWordsTest.php
--------------------------------------------------------------------------------
FOUND 0 ERRORS AND 1 WARNING AFFECTING 1 LINE
--------------------------------------------------------------------------------
 72 | WARNING | The method parameter $text is never used
    |         | (Generic.CodeAnalysis.UnusedFunctionParameter.Found)
--------------------------------------------------------------------------------


FILE: ...i-1.24.1/extensions/SemanticMediaWiki/tests/phpunit/includes/SetupTest.php
--------------------------------------------------------------------------------
FOUND 1 ERROR AFFECTING 1 LINE
--------------------------------------------------------------------------------
 156 | ERROR | Function's cyclomatic complexity (26) exceeds allowed maximum of
     |       | 10 (Generic.Metrics.CyclomaticComplexity.MaxExceeded)
--------------------------------------------------------------------------------


FILE: .../extensions/SemanticMediaWiki/tests/phpunit/includes/storage/StoreTest.php
--------------------------------------------------------------------------------
FOUND 0 ERRORS AND 1 WARNING AFFECTING 1 LINE
--------------------------------------------------------------------------------
 150 | WARNING | The method parameter $query is never used
     |         | (Generic.CodeAnalysis.UnusedFunctionParameter.Found)
--------------------------------------------------------------------------------


FILE: ...xtensions/SemanticMediaWiki/tests/phpunit/QueryPrinterRegistryTestCase.php
--------------------------------------------------------------------------------
FOUND 0 ERRORS AND 1 WARNING AFFECTING 1 LINE
--------------------------------------------------------------------------------
 1 | WARNING | A file should declare new symbols (classes, functions, constants,
   |         | etc.) and cause no other side effects, or it should execute logic with
   |         | side effects, but should not do both. The first symbol is defined on
   |         | line 24 and the first side effect is on line 103.
   |         | (PSR1.Files.SideEffects.FoundWithSymbols)
--------------------------------------------------------------------------------


FILE: ...cMediaWiki/tests/phpunit/Integration/MediaWiki/Import/TimeDataTypeTest.php
--------------------------------------------------------------------------------
FOUND 1 ERROR AFFECTING 1 LINE
--------------------------------------------------------------------------------
 39 | ERROR | Line exceeds maximum limit of 180 characters; contains 182
    |       | characters (Generic.Files.LineLength.MaxExceeded)
--------------------------------------------------------------------------------


FILE: ...iaWiki/tests/phpunit/Integration/Parser/ByJsonParserTestCaseRunnerTest.php
--------------------------------------------------------------------------------
FOUND 0 ERRORS AND 2 WARNINGS AFFECTING 2 LINES
--------------------------------------------------------------------------------
  92 | WARNING | The method parameter $debug is never used
     |         | (Generic.CodeAnalysis.UnusedFunctionParameter.Found)
 118 | WARNING | The method parameter $debug is never used
     |         | (Generic.CodeAnalysis.UnusedFunctionParameter.Found)
--------------------------------------------------------------------------------


FILE: ...-1.24.1/extensions/SemanticMediaWiki/tests/phpunit/MwDBaseUnitTestCase.php
--------------------------------------------------------------------------------
FOUND 1 ERROR AFFECTING 1 LINE
--------------------------------------------------------------------------------
 199 | ERROR | Empty CATCH statement detected
     |       | (Generic.CodeAnalysis.EmptyStatement.DetectedCATCH)
--------------------------------------------------------------------------------


FILE: ...var/www/html/mediawiki-1.24.1/extensions/SemanticMediaWiki/tests/README.md
--------------------------------------------------------------------------------
FOUND 0 ERRORS AND 1 WARNING AFFECTING 1 LINE
--------------------------------------------------------------------------------
 1 | WARNING | No PHP code was found in this file and short open tags are not
   |         | allowed by this install of PHP. This file may be using short open tags
   |         | but PHP does not allow them. (Internal.NoCodeFound)
--------------------------------------------------------------------------------

Time: 16.92 secs; Memory: 44Mb
