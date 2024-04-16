# Comparing `tmp/amazon_bedrock_haystack-0.6.0.tar.gz` & `tmp/amazon_bedrock_haystack-0.7.0.tar.gz`

## Comparing `amazon_bedrock_haystack-0.6.0.tar` & `amazon_bedrock_haystack-0.7.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/pydoc/config.yml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/src/haystack_integrations/common/amazon_bedrock/__init__.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/src/haystack_integrations/common/amazon_bedrock/errors.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/src/haystack_integrations/common/amazon_bedrock/utils.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/src/haystack_integrations/components/embedders/amazon_bedrock/__init__.py
--rw-r--r--   0        0        0    12587 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/src/haystack_integrations/components/embedders/amazon_bedrock/document_embedder.py
--rw-r--r--   0        0        0     8479 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/src/haystack_integrations/components/embedders/amazon_bedrock/text_embedder.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/src/haystack_integrations/components/generators/amazon_bedrock/__init__.py
--rw-r--r--   0        0        0    11516 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/src/haystack_integrations/components/generators/amazon_bedrock/adapters.py
--rw-r--r--   0        0        0    12313 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/src/haystack_integrations/components/generators/amazon_bedrock/generator.py
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/src/haystack_integrations/components/generators/amazon_bedrock/handlers.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/src/haystack_integrations/components/generators/amazon_bedrock/chat/__init__.py
--rw-r--r--   0        0        0    16541 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/src/haystack_integrations/components/generators/amazon_bedrock/chat/adapters.py
--rw-r--r--   0        0        0    12281 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/src/haystack_integrations/components/generators/amazon_bedrock/chat/chat_generator.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0    12165 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/tests/test_chat_generator.py
--rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/tests/test_document_embedder.py
--rw-r--r--   0        0        0    36999 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/tests/test_generator.py
--rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/tests/test_text_embedder.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/README.md
--rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.6.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1444 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/examples/chatgenerator_example.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/examples/embedders_generator_with_rag_example.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/pydoc/config.yml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/common/amazon_bedrock/__init__.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/common/amazon_bedrock/errors.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/common/amazon_bedrock/utils.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/embedders/amazon_bedrock/__init__.py
+-rw-r--r--   0        0        0    12587 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/embedders/amazon_bedrock/document_embedder.py
+-rw-r--r--   0        0        0     8479 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/embedders/amazon_bedrock/text_embedder.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/generators/amazon_bedrock/__init__.py
+-rw-r--r--   0        0        0    13329 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/generators/amazon_bedrock/adapters.py
+-rw-r--r--   0        0        0    12287 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/generators/amazon_bedrock/generator.py
+-rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/generators/amazon_bedrock/handlers.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/generators/amazon_bedrock/chat/__init__.py
+-rw-r--r--   0        0        0    23013 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/generators/amazon_bedrock/chat/adapters.py
+-rw-r--r--   0        0        0    12343 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/generators/amazon_bedrock/chat/chat_generator.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0    15641 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/tests/test_chat_generator.py
+-rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/tests/test_document_embedder.py
+-rw-r--r--   0        0        0    41832 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/tests/test_generator.py
+-rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/tests/test_text_embedder.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/README.md
+-rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/PKG-INFO
```

### Comparing `amazon_bedrock_haystack-0.6.0/pydoc/config.yml` & `amazon_bedrock_haystack-0.7.0/pydoc/config.yml`

 * *Files 6% similar despite different names*

```diff
@@ -24,11 +24,12 @@
   excerpt: Amazon Bedrock integration for Haystack
   category_slug: integrations-api
   title: Amazon Bedrock
   slug: integrations-amazon-bedrock
   order: 9
   markdown:
     descriptive_class_title: false
+    classdef_code_block: false
     descriptive_module_title: true
     add_method_class_prefix: true
     add_member_class_prefix: false
     filename: _readme_amazon_bedrock.md
```

### Comparing `amazon_bedrock_haystack-0.6.0/src/haystack_integrations/common/amazon_bedrock/errors.py` & `amazon_bedrock_haystack-0.7.0/src/haystack_integrations/common/amazon_bedrock/errors.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.6.0/src/haystack_integrations/common/amazon_bedrock/utils.py` & `amazon_bedrock_haystack-0.7.0/src/haystack_integrations/common/amazon_bedrock/utils.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.6.0/src/haystack_integrations/components/embedders/amazon_bedrock/document_embedder.py` & `amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/embedders/amazon_bedrock/document_embedder.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.6.0/src/haystack_integrations/components/embedders/amazon_bedrock/text_embedder.py` & `amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/embedders/amazon_bedrock/text_embedder.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.6.0/src/haystack_integrations/components/generators/amazon_bedrock/adapters.py` & `amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/generators/amazon_bedrock/adapters.py`

 * *Files 8% similar despite different names*

```diff
@@ -135,14 +135,63 @@
 
         :param chunk: The streaming chunk.
         :returns: A string token.
         """
         return chunk.get("completion", "")
 
 
+class MistralAdapter(BedrockModelAdapter):
+    """
+    Adapter for the Mistral models.
+    """
+
+    def prepare_body(self, prompt: str, **inference_kwargs) -> Dict[str, Any]:
+        """
+        Prepares the body for the Mistral model
+
+        :param prompt: The prompt to be sent to the model.
+        :param inference_kwargs: Additional keyword arguments passed to the handler.
+        :returns: A dictionary with the following keys:
+            - `prompt`: The prompt to be sent to the model.
+            - specified inference parameters.
+        """
+        default_params: Dict[str, Any] = {
+            "max_tokens": self.max_length,
+            "stop": [],
+            "temperature": None,
+            "top_p": None,
+            "top_k": None,
+        }
+        params = self._get_params(inference_kwargs, default_params)
+        # Add the instruction tag to the prompt if it's not already there
+        formatted_prompt = f"<s>[INST] {prompt} [/INST]" if "INST" not in prompt else prompt
+        return {"prompt": formatted_prompt, **params}
+
+    def _extract_completions_from_response(self, response_body: Dict[str, Any]) -> List[str]:
+        """
+        Extracts the responses from the Amazon Bedrock response.
+
+        :param response_body: The response body from the Amazon Bedrock request.
+        :returns: A list of string responses.
+        """
+        return [output.get("text", "") for output in response_body.get("outputs", [])]
+
+    def _extract_token_from_stream(self, chunk: Dict[str, Any]) -> str:
+        """
+        Extracts the token from a streaming chunk.
+
+        :param chunk: The streaming chunk.
+        :returns: A string token.
+        """
+        chunk_list = chunk.get("outputs", [])
+        if chunk_list:
+            return chunk_list[0].get("text", "")
+        return ""
+
+
 class CohereCommandAdapter(BedrockModelAdapter):
     """
     Adapter for the Cohere Command model.
     """
 
     def prepare_body(self, prompt: str, **inference_kwargs) -> Dict[str, Any]:
         """
```

### Comparing `amazon_bedrock_haystack-0.6.0/src/haystack_integrations/components/generators/amazon_bedrock/generator.py` & `amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/generators/amazon_bedrock/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from .adapters import (
     AI21LabsJurassic2Adapter,
     AmazonTitanAdapter,
     AnthropicClaudeAdapter,
     BedrockModelAdapter,
     CohereCommandAdapter,
     MetaLlama2ChatAdapter,
+    MistralAdapter,
 )
 from .handlers import (
     DefaultPromptHandler,
     DefaultTokenStreamingHandler,
     TokenStreamingHandler,
 )
 
@@ -54,14 +55,15 @@
 
     SUPPORTED_MODEL_PATTERNS: ClassVar[Dict[str, Type[BedrockModelAdapter]]] = {
         r"amazon.titan-text.*": AmazonTitanAdapter,
         r"ai21.j2.*": AI21LabsJurassic2Adapter,
         r"cohere.command.*": CohereCommandAdapter,
         r"anthropic.claude.*": AnthropicClaudeAdapter,
         r"meta.llama2.*": MetaLlama2ChatAdapter,
+        r"mistral.*": MistralAdapter,
     }
 
     def __init__(
         self,
         model: str,
         aws_access_key_id: Optional[Secret] = Secret.from_env_var("AWS_ACCESS_KEY_ID", strict=False),  # noqa: B008
         aws_secret_access_key: Optional[Secret] = Secret.from_env_var(  # noqa: B008
@@ -120,16 +122,15 @@
 
         model_input_kwargs = kwargs
         # We pop the model_max_length as it is not sent to the model but used to truncate the prompt if needed
         model_max_length = kwargs.get("model_max_length", 4096)
 
         # Truncate prompt if prompt tokens > model_max_length-max_length
         # (max_length is the length of the generated text)
-        # It is hard to determine which tokenizer to use for the SageMaker model
-        # so we use GPT2 tokenizer which will likely provide good token count approximation
+        # we use GPT2 tokenizer which will likely provide good token count approximation
         self.prompt_handler = DefaultPromptHandler(
             tokenizer="gpt2",
             model_max_length=model_max_length,
             max_length=self.max_length or 100,
         )
 
         model_adapter_cls = self.get_model_adapter(model=model)
```

### Comparing `amazon_bedrock_haystack-0.6.0/src/haystack_integrations/components/generators/amazon_bedrock/handlers.py` & `amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/generators/amazon_bedrock/handlers.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.6.0/src/haystack_integrations/components/generators/amazon_bedrock/chat/adapters.py` & `amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/generators/amazon_bedrock/chat/adapters.py`

 * *Files 13% similar despite different names*

```diff
@@ -267,14 +267,168 @@
         Convert a ChatMessage to a dictionary with the content and role fields.
         :param m: The ChatMessage to convert.
         :return: The dictionary with the content and role fields.
         """
         return {"content": [{"type": "text", "text": m.content}], "role": m.role.value}
 
 
+class MistralChatAdapter(BedrockModelChatAdapter):
+    """
+    Model adapter for the Mistral chat model.
+    """
+
+    chat_template = """
+    {% if messages[0]['role'] == 'system' %}
+        {% set loop_messages = messages[1:] %}
+        {% set system_message = messages[0]['content'] %}
+    {% else %}
+        {% set loop_messages = messages %}
+        {% set system_message = false %}
+    {% endif %}
+    {{bos_token}}
+    {% for message in loop_messages %}
+        {% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}
+            {{ raise_exception('Conversation roles must alternate user/assistant/user/assistant/...') }}
+        {% endif %}
+        {% if loop.index0 == 0 and system_message != false %}
+            {% set content = system_message + '\n' + message['content'] %}
+        {% else %}
+            {% set content = message['content'] %}
+        {% endif %}
+        {% if message['role'] == 'user' %}
+            {{ '[INST] ' + content.strip() + ' [/INST]' }}
+        {% elif message['role'] == 'assistant' %}
+            {{ content.strip() + eos_token }}
+        {% endif %}
+    {% endfor %}
+    """
+    chat_template = "".join(line.strip() for line in chat_template.splitlines())
+
+    # the above template was designed to match https://docs.mistral.ai/models/#chat-template
+    # and to support system messages, otherwise we could use the default mistral chat template
+    # available on HF infrastructure
+
+    # https://docs.aws.amazon.com/bedrock/latest/userguide/model-parameters-anthropic-claude-messages.html
+    ALLOWED_PARAMS: ClassVar[List[str]] = [
+        "max_tokens",
+        "safe_prompt",
+        "random_seed",
+        "temperature",
+        "top_p",
+    ]
+
+    def __init__(self, generation_kwargs: Dict[str, Any]):
+        """
+        Initializes the Mistral chat adapter.
+
+        :param generation_kwargs: The generation kwargs.
+        """
+        super().__init__(generation_kwargs)
+
+        # We pop the model_max_length as it is not sent to the model
+        # but used to truncate the prompt if needed
+        # Mistral has a limit of at least 32000 tokens
+        model_max_length = self.generation_kwargs.pop("model_max_length", 32000)
+
+        # Use `mistralai/Mistral-7B-v0.1` as tokenizer, all mistral models likely use the same tokenizer
+        # a) we should get good estimates for the prompt length
+        # b) we can use apply_chat_template with the template above to delineate ChatMessages
+        tokenizer: PreTrainedTokenizer = AutoTokenizer.from_pretrained("mistralai/Mistral-7B-Instruct-v0.1")
+        self.prompt_handler = DefaultPromptHandler(
+            tokenizer=tokenizer,
+            model_max_length=model_max_length,
+            max_length=self.generation_kwargs.get("max_gen_len") or 512,
+        )
+
+    def prepare_body(self, messages: List[ChatMessage], **inference_kwargs) -> Dict[str, Any]:
+        """
+        Prepares the body for the Mistral request.
+
+        :param messages: The chat messages to package into the request.
+        :param inference_kwargs: Additional inference kwargs to use.
+        :returns: The prepared body.
+        """
+        default_params = {
+            "max_tokens": self.generation_kwargs.get("max_tokens") or 512,  # max_tokens is required
+        }
+        # replace stop_words from inference_kwargs with stop, as this is Mistral specific parameter
+        stop_words = inference_kwargs.pop("stop_words", [])
+        if stop_words:
+            inference_kwargs["stop"] = stop_words
+        params = self._get_params(inference_kwargs, default_params, self.ALLOWED_PARAMS)
+        body = {"prompt": self.prepare_chat_messages(messages=messages), **params}
+        return body
+
+    def prepare_chat_messages(self, messages: List[ChatMessage]) -> str:
+        """
+        Prepares the chat messages for the Mistral request.
+
+        :param messages: The chat messages to prepare.
+        :returns: The prepared chat messages as a string.
+        """
+        # it would be great to use the default mistral chat template, but it doesn't support system messages
+        # the class variable defined chat_template is a workaround to support system messages
+        # default is https://huggingface.co/mistralai/Mixtral-8x7B-Instruct-v0.1/blob/main/tokenizer_config.json
+        # but we'll use our custom chat template
+        prepared_prompt: str = self.prompt_handler.tokenizer.apply_chat_template(
+            conversation=[self.to_openai_format(m) for m in messages], tokenize=False, chat_template=self.chat_template
+        )
+        return self._ensure_token_limit(prepared_prompt)
+
+    def to_openai_format(self, m: ChatMessage) -> Dict[str, Any]:
+        """
+        Convert the message to the format expected by OpenAI's Chat API.
+        See the [API reference](https://platform.openai.com/docs/api-reference/chat/create) for details.
+
+        :returns: A dictionary with the following key:
+            - `role`
+            - `content`
+            - `name` (optional)
+        """
+        msg = {"role": m.role.value, "content": m.content}
+        if m.name:
+            msg["name"] = m.name
+        return msg
+
+    def check_prompt(self, prompt: str) -> Dict[str, Any]:
+        """
+        Checks the prompt length and resizes it if necessary. If the prompt is too long, it will be truncated.
+
+        :param prompt: The prompt to check.
+        :returns: A dictionary containing the resized prompt and additional information.
+        """
+        return self.prompt_handler(prompt)
+
+    def _extract_messages_from_response(self, response_body: Dict[str, Any]) -> List[ChatMessage]:
+        """
+        Extracts the messages from the response body.
+
+        :param response_body: The response body.
+        :return: The extracted ChatMessage list.
+        """
+        messages: List[ChatMessage] = []
+        responses = response_body.get("outputs", [])
+        for response in responses:
+            meta = {k: v for k, v in response.items() if k not in ["text"]}
+            messages.append(ChatMessage.from_assistant(response["text"], meta=meta))
+        return messages
+
+    def _extract_token_from_stream(self, chunk: Dict[str, Any]) -> str:
+        """
+        Extracts the token from a streaming chunk.
+
+        :param chunk: The streaming chunk.
+        :returns: The extracted token.
+        """
+        response_chunk = chunk.get("outputs", [])
+        if response_chunk:
+            return response_chunk[0].get("text", "")
+        return ""
+
+
 class MetaLlama2ChatAdapter(BedrockModelChatAdapter):
     """
     Model adapter for the Meta Llama 2 models.
     """
 
     # https://docs.aws.amazon.com/bedrock/latest/userguide/model-parameters-meta.html
     ALLOWED_PARAMS: ClassVar[List[str]] = ["max_gen_len", "temperature", "top_p"]
```

### Comparing `amazon_bedrock_haystack-0.6.0/src/haystack_integrations/components/generators/amazon_bedrock/chat/chat_generator.py` & `amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/generators/amazon_bedrock/chat/chat_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from haystack_integrations.common.amazon_bedrock.errors import (
     AmazonBedrockConfigurationError,
     AmazonBedrockInferenceError,
 )
 from haystack_integrations.common.amazon_bedrock.utils import get_aws_session
 
-from .adapters import AnthropicClaudeChatAdapter, BedrockModelChatAdapter, MetaLlama2ChatAdapter
+from .adapters import AnthropicClaudeChatAdapter, BedrockModelChatAdapter, MetaLlama2ChatAdapter, MistralChatAdapter
 
 logger = logging.getLogger(__name__)
 
 
 @component
 class AmazonBedrockChatGenerator:
     """
@@ -46,14 +46,15 @@
     If you prefer non-streaming mode, simply remove the `streaming_callback` parameter, capture the return value of the
     component's run method and the `AmazonBedrockChatGenerator` will return the response in a non-streaming mode.
     """
 
     SUPPORTED_MODEL_PATTERNS: ClassVar[Dict[str, Type[BedrockModelChatAdapter]]] = {
         r"anthropic.claude.*": AnthropicClaudeChatAdapter,
         r"meta.llama2.*": MetaLlama2ChatAdapter,
+        r"mistral.*": MistralChatAdapter,
     }
 
     def __init__(
         self,
         model: str,
         aws_access_key_id: Optional[Secret] = Secret.from_env_var(["AWS_ACCESS_KEY_ID"], strict=False),  # noqa: B008
         aws_secret_access_key: Optional[Secret] = Secret.from_env_var(  # noqa: B008
```

### Comparing `amazon_bedrock_haystack-0.6.0/tests/conftest.py` & `amazon_bedrock_haystack-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.6.0/tests/test_chat_generator.py` & `amazon_bedrock_haystack-0.7.0/tests/test_chat_generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,18 +5,24 @@
 from haystack.dataclasses import ChatMessage, ChatRole, StreamingChunk
 
 from haystack_integrations.components.generators.amazon_bedrock import AmazonBedrockChatGenerator
 from haystack_integrations.components.generators.amazon_bedrock.chat.adapters import (
     AnthropicClaudeChatAdapter,
     BedrockModelChatAdapter,
     MetaLlama2ChatAdapter,
+    MistralChatAdapter,
 )
 
 KLASS = "haystack_integrations.components.generators.amazon_bedrock.chat.chat_generator.AmazonBedrockChatGenerator"
 MODELS_TO_TEST = ["anthropic.claude-3-sonnet-20240229-v1:0", "anthropic.claude-v2:1", "meta.llama2-13b-chat-v1"]
+MISTRAL_MODELS = [
+    "mistral.mistral-7b-instruct-v0:2",
+    "mistral.mixtral-8x7b-instruct-v0:1",
+    "mistral.mistral-large-2402-v1:0",
+]
 
 
 def test_to_dict(mock_boto3_session):
     """
     Test that the to_dict method returns the correct dictionary without aws credentials
     """
     generator = AmazonBedrockChatGenerator(
@@ -172,14 +178,88 @@
         body = layer.prepare_body(
             [ChatMessage.from_user(prompt)], top_p=0.8, top_k=5, max_tokens_to_sample=69, stop_sequences=["CUSTOM_STOP"]
         )
 
         assert body == expected_body
 
 
+class TestMistralAdapter:
+    def test_prepare_body_with_default_params(self) -> None:
+        layer = MistralChatAdapter(generation_kwargs={})
+        prompt = "Hello, how are you?"
+        expected_body = {
+            "max_tokens": 512,
+            "prompt": "<s>[INST] Hello, how are you? [/INST]",
+        }
+
+        body = layer.prepare_body([ChatMessage.from_user(prompt)])
+
+        assert body == expected_body
+
+    def test_prepare_body_with_custom_inference_params(self) -> None:
+        layer = MistralChatAdapter(generation_kwargs={"temperature": 0.7, "top_p": 0.8, "top_k": 4})
+        prompt = "Hello, how are you?"
+        expected_body = {
+            "prompt": "<s>[INST] Hello, how are you? [/INST]",
+            "max_tokens": 512,
+            "temperature": 0.7,
+            "top_p": 0.8,
+        }
+
+        body = layer.prepare_body([ChatMessage.from_user(prompt)], top_p=0.8, top_k=5, max_tokens_to_sample=69)
+
+        assert body == expected_body
+
+    def test_mistral_chat_template_correct_order(self):
+        layer = MistralChatAdapter(generation_kwargs={})
+        layer.prepare_body([ChatMessage.from_user("A"), ChatMessage.from_assistant("B"), ChatMessage.from_user("C")])
+        layer.prepare_body([ChatMessage.from_system("A"), ChatMessage.from_user("B"), ChatMessage.from_assistant("C")])
+
+    def test_mistral_chat_template_incorrect_order(self):
+        layer = MistralChatAdapter(generation_kwargs={})
+        try:
+            layer.prepare_body([ChatMessage.from_assistant("B"), ChatMessage.from_assistant("C")])
+            msg = "Expected TemplateError"
+            raise AssertionError(msg)
+        except Exception as e:
+            assert "Conversation roles must alternate user/assistant/" in str(e)
+
+        try:
+            layer.prepare_body([ChatMessage.from_user("A"), ChatMessage.from_user("B")])
+            msg = "Expected TemplateError"
+            raise AssertionError(msg)
+        except Exception as e:
+            assert "Conversation roles must alternate user/assistant/" in str(e)
+
+        try:
+            layer.prepare_body([ChatMessage.from_system("A"), ChatMessage.from_system("B")])
+            msg = "Expected TemplateError"
+            raise AssertionError(msg)
+        except Exception as e:
+            assert "Conversation roles must alternate user/assistant/" in str(e)
+
+    @pytest.mark.parametrize("model_name", MISTRAL_MODELS)
+    @pytest.mark.integration
+    def test_default_inference_params(self, model_name, chat_messages):
+        client = AmazonBedrockChatGenerator(model=model_name)
+        response = client.run(chat_messages)
+
+        assert "replies" in response, "Response does not contain 'replies' key"
+        replies = response["replies"]
+        assert isinstance(replies, list), "Replies is not a list"
+        assert len(replies) > 0, "No replies received"
+
+        first_reply = replies[0]
+        assert isinstance(first_reply, ChatMessage), "First reply is not a ChatMessage instance"
+        assert first_reply.content, "First reply has no content"
+        assert ChatMessage.is_from(first_reply, ChatRole.ASSISTANT), "First reply is not from the assistant"
+        assert "paris" in first_reply.content.lower(), "First reply does not contain 'paris'"
+        assert first_reply.meta, "First reply has no metadata"
+
+
 @pytest.fixture
 def chat_messages():
     messages = [
         ChatMessage.from_system("\\nYou are a helpful assistant, be super brief in your responses."),
         ChatMessage.from_user("What's the capital of France?"),
     ]
     return messages
```

### Comparing `amazon_bedrock_haystack-0.6.0/tests/test_document_embedder.py` & `amazon_bedrock_haystack-0.7.0/tests/test_document_embedder.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.6.0/tests/test_generator.py` & `amazon_bedrock_haystack-0.7.0/tests/test_generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from haystack_integrations.components.generators.amazon_bedrock.adapters import (
     AI21LabsJurassic2Adapter,
     AmazonTitanAdapter,
     AnthropicClaudeAdapter,
     BedrockModelAdapter,
     CohereCommandAdapter,
     MetaLlama2ChatAdapter,
+    MistralAdapter,
 )
 
 
 def test_to_dict(mock_boto3_session):
     """
     Test that the to_dict method returns the correct dictionary without aws credentials
     """
@@ -363,14 +364,147 @@
         adapter = AnthropicClaudeAdapter(model_kwargs={}, max_length=99)
         expected_responses = [""]
         assert adapter.get_stream_responses(stream_mock, stream_handler_mock) == expected_responses
 
         stream_handler_mock.assert_not_called()
 
 
+class TestMistralAdapter:
+    def test_prepare_body_with_default_params(self) -> None:
+        layer = MistralAdapter(model_kwargs={}, max_length=99)
+        prompt = "Hello, how are you?"
+        expected_body = {"prompt": "<s>[INST] Hello, how are you? [/INST]", "max_tokens": 99, "stop": []}
+
+        body = layer.prepare_body(prompt)
+        assert body == expected_body
+
+    def test_prepare_body_with_custom_inference_params(self) -> None:
+        layer = MistralAdapter(model_kwargs={}, max_length=99)
+        prompt = "Hello, how are you?"
+        expected_body = {
+            "prompt": "<s>[INST] Hello, how are you? [/INST]",
+            "max_tokens": 50,
+            "stop": ["CUSTOM_STOP"],
+            "temperature": 0.7,
+            "top_p": 0.8,
+            "top_k": 5,
+        }
+
+        body = layer.prepare_body(
+            prompt,
+            temperature=0.7,
+            top_p=0.8,
+            top_k=5,
+            max_tokens=50,
+            stop=["CUSTOM_STOP"],
+            unknown_arg="unknown_value",
+        )
+
+        assert body == expected_body
+
+    def test_prepare_body_with_model_kwargs(self) -> None:
+        layer = MistralAdapter(
+            model_kwargs={
+                "temperature": 0.7,
+                "top_p": 0.8,
+                "top_k": 5,
+                "max_tokens": 50,
+                "stop": ["CUSTOM_STOP"],
+                "unknown_arg": "unknown_value",
+            },
+            max_length=99,
+        )
+        prompt = "Hello, how are you?"
+        expected_body = {
+            "prompt": "<s>[INST] Hello, how are you? [/INST]",
+            "max_tokens": 50,
+            "stop": ["CUSTOM_STOP"],
+            "temperature": 0.7,
+            "top_p": 0.8,
+            "top_k": 5,
+        }
+
+        body = layer.prepare_body(prompt)
+
+        assert body == expected_body
+
+    def test_prepare_body_with_model_kwargs_and_custom_inference_params(self) -> None:
+        layer = MistralAdapter(
+            model_kwargs={
+                "temperature": 0.6,
+                "top_p": 0.7,
+                "top_k": 4,
+                "max_tokens": 49,
+                "stop": ["CUSTOM_STOP_MODEL_KWARGS"],
+            },
+            max_length=99,
+        )
+        prompt = "Hello, how are you?"
+        expected_body = {
+            "prompt": "<s>[INST] Hello, how are you? [/INST]",
+            "max_tokens": 50,
+            "stop": ["CUSTOM_STOP_MODEL_KWARGS"],
+            "temperature": 0.7,
+            "top_p": 0.8,
+            "top_k": 5,
+        }
+
+        body = layer.prepare_body(prompt, temperature=0.7, top_p=0.8, top_k=5, max_tokens=50)
+
+        assert body == expected_body
+
+    def test_get_responses(self) -> None:
+        adapter = MistralAdapter(model_kwargs={}, max_length=99)
+        response_body = {"outputs": [{"text": "This is a single response."}]}
+        expected_responses = ["This is a single response."]
+        assert adapter.get_responses(response_body) == expected_responses
+
+    def test_get_stream_responses(self) -> None:
+        stream_mock = MagicMock()
+        stream_handler_mock = MagicMock()
+
+        stream_mock.__iter__.return_value = [
+            {"chunk": {"bytes": b'{"outputs": [{"text": " This"}]}'}},
+            {"chunk": {"bytes": b'{"outputs": [{"text": " is"}]}'}},
+            {"chunk": {"bytes": b'{"outputs": [{"text": " a"}]}'}},
+            {"chunk": {"bytes": b'{"outputs": [{"text": " single"}]}'}},
+            {"chunk": {"bytes": b'{"outputs": [{"text": " response."}]}'}},
+        ]
+
+        stream_handler_mock.side_effect = lambda token_received, **kwargs: token_received
+
+        adapter = MistralAdapter(model_kwargs={}, max_length=99)
+        expected_responses = ["This is a single response."]
+        assert adapter.get_stream_responses(stream_mock, stream_handler_mock) == expected_responses
+
+        stream_handler_mock.assert_has_calls(
+            [
+                call(" This", event_data={"outputs": [{"text": " This"}]}),
+                call(" is", event_data={"outputs": [{"text": " is"}]}),
+                call(" a", event_data={"outputs": [{"text": " a"}]}),
+                call(" single", event_data={"outputs": [{"text": " single"}]}),
+                call(" response.", event_data={"outputs": [{"text": " response."}]}),
+            ]
+        )
+
+    def test_get_stream_responses_empty(self) -> None:
+        stream_mock = MagicMock()
+        stream_handler_mock = MagicMock()
+
+        stream_mock.__iter__.return_value = []
+
+        stream_handler_mock.side_effect = lambda token_received, **kwargs: token_received
+
+        adapter = MistralAdapter(model_kwargs={}, max_length=99)
+        expected_responses = [""]
+        assert adapter.get_stream_responses(stream_mock, stream_handler_mock) == expected_responses
+
+        stream_handler_mock.assert_not_called()
+
+
 class TestCohereCommandAdapter:
     def test_prepare_body_with_default_params(self) -> None:
         layer = CohereCommandAdapter(model_kwargs={}, max_length=99)
         prompt = "Hello, how are you?"
         expected_body = {"prompt": "Hello, how are you?", "max_tokens": 99}
 
         body = layer.prepare_body(prompt)
```

### Comparing `amazon_bedrock_haystack-0.6.0/tests/test_text_embedder.py` & `amazon_bedrock_haystack-0.7.0/tests/test_text_embedder.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.6.0/.gitignore` & `amazon_bedrock_haystack-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.6.0/LICENSE.txt` & `amazon_bedrock_haystack-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.6.0/README.md` & `amazon_bedrock_haystack-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.6.0/pyproject.toml` & `amazon_bedrock_haystack-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -92,20 +92,20 @@
 
 all = [
   "style",
   "typing",
 ]
 
 [tool.black]
-target-version = ["py37"]
+target-version = ["py38"]
 line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
-target-version = "py37"
+target-version = "py38"
 line-length = 120
 select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
```

### Comparing `amazon_bedrock_haystack-0.6.0/PKG-INFO` & `amazon_bedrock_haystack-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: amazon-bedrock-haystack
-Version: 0.6.0
+Version: 0.7.0
 Summary: An integration of Amazon Bedrock as an AmazonBedrockGenerator component.
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/amazon_bedrock#readme
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/amazon_bedrock
 Author-email: deepset GmbH <info@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
```

