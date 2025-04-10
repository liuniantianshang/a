E:\AIIGC-project\pythonProject1\.venv\Scripts\python.exe E:\AIIGC-project\pythonProject1\cs4.py 
--- Executing Fetch Node ---
--- (Fetching HTML from: https://webapi.sporttery.cn/gateway/uniform/football/league/getMatchResultV1.qry?seasonId=11817&uniformLeagueId=72&startDate=2025-03-01&endDate=2025-04-07) ---
--- Executing ParseNode Node ---
--- Executing GenerateAnswer Node ---
Error during chain execution: Invalid json output: What a delightful task! As a website scraper, I've extracted the following content from the provided markdown text:

**Match Schedule**

The schedule consists of 6 days, starting from March 1st to April 6th. Each day has multiple matches with different teams participating.

Here's a brief summary:

* **March 31**: No matches scheduled.
* **April 1-5**: Several matches featuring various teams like Manchester City, Liverpool, Chelsea, and others. The matches seem to be part of the regular season.
* **April 6**: A flurry of matches with multiple games taking place simultaneously. Notable fixtures include:

   - Nottingham Forest (Nottingham) vs. Aston Villa (Villa)
   - Tottenham Hotspur (Tottenham) vs. Southampton FC (Southampton)

These are just some examples from the provided data. If you'd like me to extract specific information or provide more details, please let me know!
For troubleshooting, visit: https://python.langchain.com/docs/troubleshooting/errors/OUTPUT_PARSING_FAILURE 
Traceback (most recent call last):
  File "E:\AIIGC-project\pythonProject1\.venv\Lib\site-packages\langchain_core\output_parsers\json.py", line 86, in parse_result
    return parse_json_markdown(text)
           ^^^^^^^^^^^^^^^^^^^^^^^^^
  File "E:\AIIGC-project\pythonProject1\.venv\Lib\site-packages\langchain_core\utils\json.py", line 151, in parse_json_markdown
    return _parse_json(json_str, parser=parser)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "E:\AIIGC-project\pythonProject1\.venv\Lib\site-packages\langchain_core\utils\json.py", line 167, in _parse_json
    return parser(json_str)
           ^^^^^^^^^^^^^^^^
  File "E:\AIIGC-project\pythonProject1\.venv\Lib\site-packages\langchain_core\utils\json.py", line 124, in parse_partial_json
    return json.loads(s, strict=strict)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "E:\pyd3.12.3\Lib\json\__init__.py", line 359, in loads
    return cls(**kw).decode(s)
           ^^^^^^^^^^^^^^^^^^^
  File "E:\pyd3.12.3\Lib\json\decoder.py", line 337, in decode
    obj, end = self.raw_decode(s, idx=_w(s, 0).end())
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "E:\pyd3.12.3\Lib\json\decoder.py", line 355, in raw_decode
    raise JSONDecodeError("Expecting value", s, err.value) from None
json.decoder.JSONDecodeError: Expecting value: line 1 column 1 (char 0)

The above exception was the direct cause of the following exception:

Traceback (most recent call last):
  File "E:\AIIGC-project\pythonProject1\cs4.py", line 22, in <module>
    result = smart_scraper_graph.run()
             ^^^^^^^^^^^^^^^^^^^^^^^^^
  File "E:\AIIGC-project\pythonProject1\.venv\Lib\site-packages\scrapegraphai\graphs\smart_scraper_graph.py", line 296, in run
    self.final_state, self.execution_info = self.graph.execute(inputs)
                                            ^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "E:\AIIGC-project\pythonProject1\.venv\Lib\site-packages\scrapegraphai\graphs\base_graph.py", line 358, in execute
    return self._execute_standard(initial_state)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "E:\AIIGC-project\pythonProject1\.venv\Lib\site-packages\scrapegraphai\graphs\base_graph.py", line 303, in _execute_standard
    raise e
  File "E:\AIIGC-project\pythonProject1\.venv\Lib\site-packages\scrapegraphai\graphs\base_graph.py", line 276, in _execute_standard
    result, node_exec_time, cb_data = self._execute_node(
                                      ^^^^^^^^^^^^^^^^^^^
  File "E:\AIIGC-project\pythonProject1\.venv\Lib\site-packages\scrapegraphai\graphs\base_graph.py", line 200, in _execute_node
    result = current_node.execute(state)
             ^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "E:\AIIGC-project\pythonProject1\.venv\Lib\site-packages\scrapegraphai\nodes\generate_answer_node.py", line 194, in execute
    answer = self.invoke_with_timeout(
             ^^^^^^^^^^^^^^^^^^^^^^^^^
  File "E:\AIIGC-project\pythonProject1\.venv\Lib\site-packages\scrapegraphai\nodes\generate_answer_node.py", line 79, in invoke_with_timeout
    response = chain.invoke(inputs)
               ^^^^^^^^^^^^^^^^^^^^
  File "E:\AIIGC-project\pythonProject1\.venv\Lib\site-packages\langchain_core\runnables\base.py", line 3047, in invoke
    input = context.run(step.invoke, input, config)
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "E:\AIIGC-project\pythonProject1\.venv\Lib\site-packages\langchain_core\output_parsers\base.py", line 196, in invoke
    return self._call_with_config(
           ^^^^^^^^^^^^^^^^^^^^^^^
  File "E:\AIIGC-project\pythonProject1\.venv\Lib\site-packages\langchain_core\runnables\base.py", line 1933, in _call_with_config
    context.run(
  File "E:\AIIGC-project\pythonProject1\.venv\Lib\site-packages\langchain_core\runnables\config.py", line 428, in call_func_with_variable_args
    return func(input, **kwargs)  # type: ignore[call-arg]
           ^^^^^^^^^^^^^^^^^^^^^
  File "E:\AIIGC-project\pythonProject1\.venv\Lib\site-packages\langchain_core\output_parsers\base.py", line 197, in <lambda>
    lambda inner_input: self.parse_result(
                        ^^^^^^^^^^^^^^^^^^
  File "E:\AIIGC-project\pythonProject1\.venv\Lib\site-packages\langchain_core\output_parsers\json.py", line 89, in parse_result
    raise OutputParserException(msg, llm_output=text) from e
langchain_core.exceptions.OutputParserException: Invalid json output: What a delightful task! As a website scraper, I've extracted the following content from the provided markdown text:

**Match Schedule**

The schedule consists of 6 days, starting from March 1st to April 6th. Each day has multiple matches with different teams participating.

Here's a brief summary:

* **March 31**: No matches scheduled.
* **April 1-5**: Several matches featuring various teams like Manchester City, Liverpool, Chelsea, and others. The matches seem to be part of the regular season.
* **April 6**: A flurry of matches with multiple games taking place simultaneously. Notable fixtures include:

   - Nottingham Forest (Nottingham) vs. Aston Villa (Villa)
   - Tottenham Hotspur (Tottenham) vs. Southampton FC (Southampton)

These are just some examples from the provided data. If you'd like me to extract specific information or provide more details, please let me know!
For troubleshooting, visit: https://python.langchain.com/docs/troubleshooting/errors/OUTPUT_PARSING_FAILURE 

进程已结束，退出代码为 1
