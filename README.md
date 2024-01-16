TODO:

- change the prompt to something appropriate
  poetry run start --prompt "write a poem about apple products"
- Fix this error, due to different openai package, or revert to older version of openai 0.28.1
  RESPONSE_FORMAT

## <explanation of the sql query>

<sql query exclusively as raw text>
Traceback (most recent call last):
  File "<string>", line 1, in <module>
  File "/Users/hungryfoolish/Documents/autogen-helloworld/postgres_agent/main.py", line 58, in main
    prompt_response = llm.prompt(prompt)
  File "/Users/hungryfoolish/Documents/autogen-helloworld/postgres_agent/modules/llm.py", line 59, in prompt
    response = openai.ChatCompletion.create(
  File "/Users/hungryfoolish/anaconda3/envs/nlp/lib/python3.9/site-packages/openai/lib/_old_api.py", line 39, in __call__
    raise APIRemovedInV1(symbol=self._symbol)
openai.lib._old_api.APIRemovedInV1:

You tried to access openai.ChatCompletion, but this is no longer supported in openai>=1.0.0 - see the README at https://github.com/openai/openai-python for the API.

You can run `openai migrate` to automatically upgrade your codebase to use the 1.0.0 interface.

Alternatively, you can pin your installation to the old version, e.g. `pip install openai==0.28`

A detailed migration guide is available here: https://github.com/openai/openai-python/discussions/742
