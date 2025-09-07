---
title: 2025-09-06Why language models hallucinate
tags: 新建,模板,小书匠
category: /小书匠/日记/2025-09
grammar_cjkRuby: true
---

OpenAI 揭秘：AI为什么会一本正经地胡说八道？ OpenAI 最近发表了一篇名为《语言模型为何会产生幻觉》(Why Language Models Hallucinate) 的文章，深入解释了 AI “幻觉”产生的根本原因，并提出了减少这种现象的解决方案。 规则的“锅”：AI 被鼓励去猜测，而非承认无知 文章指出，大语言模型之所以会产生“幻觉”，是因为我们现有的训练和评估方式存在一个根本性问题：它奖励猜测，而不是鼓励模型承认自己的不确定性。 大多数评估体系衡量模型表现的方式，都无形中让模型养成了“猜答案”的习惯。当模型的评分标准只基于准确性时，它为了拿高分，自然会倾向于在不确定的时候蒙一个答案，而不是诚实地回答“我不知道”。 问题的根源：来自“预训练”阶段的先天不足 这种“爱猜测”的习惯，其实在模型的“学前教育”阶段，也就是 预训练 (pretraining) 过程中，就已经埋下了种子。 在预训练期间，模型通过预测海量文本中的下一个词来进行学习。但问题在于，这些学习材料并没有为每一句话贴上“真”或“假”的标签。这使得模型很难区分哪些是有效陈述，哪些是无效信息。 这个挑战在处理那些偶然出现的、低频事实时尤其突出。比如，某个特定宠物的生日是哪天？这类信息无法单靠语言模式来预测，模型只能去“编造”，而这正是幻觉的直接来源。 未来的出路：教会AI保持“诚实” 研究人员总结道，要解决幻觉问题，就必须更新那些只看重准确率的评估方法，让新的评分机制不再鼓励猜测。如果主流的评估“排行榜”继续奖励那些侥幸猜对的行为，那么模型就会继续学习并依赖猜测。 他们强调，幻觉并非AI不可避免的缺陷。语言模型完全有能力在不确定的时候选择“弃权”，而不是胡说八道。我们需要做的，是创造一个能鼓励这种“诚实”行为的环境和规则。
<!--StartFragment-->

<!--StartFragment-->
<div class="@container w-full max-w-container @md:shaded-container:!px-0">
  <div class="relative w-full">
    <div class="@container multi-columns:px-0 @md:shaded-container:!px-0 grid w-full grid-cols-12">
      <div class="col-span-12 @md:col-span-10 @md:col-start-2 @lg:col-span-8 @lg:col-start-3">
        <div class="relative flex flex-col items-center text-center">
          <h1 class="text-h1 max-w-[62.5rem] text-primary-100 text-balance scroll-mt-[calc(var(--header-h)+var(--toc-button-h))]">Why language models hallucinate</h1>
          <div class="mt-md min-h-sm flex justify-between">
            <div class="gap-xs flex flex-row flex-wrap items-start justify-center items-center"><a href="https://cdn.openai.com/pdf/d04913be-3f6f-4d2b-b283-ff432ef4aaa5/why-language-models-hallucinate.pdf"
              class="transition duration-short ease-curve-a rounded-[2.5rem] text-nowrap min-h-md flex items-center justify-center gap-[0.3em] text-cta focus:outline focus:outline-1 outline-offset-2 h-[2.5rem] bg-primary-4 text-primary-100 px-xs hover:bg-primary-12 disabled:bg-primary-4 disabled:text-primary-60 focus:bg-primary-12 focus:outline-primary-12"
              target="_blank" referrerpolicy="no-referrer-when-downgrade" data-analytics="why-language-models-hallucinate-layout-article-cta">Read the paper<svg width="11" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M1.70985 4.5H7.7804M7.7804 4.5V10.5705M7.7804 4.5L0.780396 11.5" stroke="currentColor" stroke-width="1.3" stroke-linecap="round" stroke-linejoin="round"></path></svg><span class="sr-only">(opens in a new window)</span></a>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="relative z-0 grid grid-cols-12 mt-lg @md:mt-xl">
      <div class="col-span-12 @md:col-span-10 @md:col-start-2">
        <div class="col-span-12 overflow-hidden">
          <div class="w-full mx-auto ease-curve-c duration-normal transition-opacity max-w-container-desktop relative min-h-0">
            <div class="relative h-full min-h-0 w-full">
              <div class="h-full w-full">
                <div class="group relative h-full w-full overflow-hidden rounded-md aspect-16/9 ease-curve-d duration-normal bg-transparent transition-[background]">
                  <img alt="Abstract image with sweeping gradients of teal, blue, and lavender, blending diagonally across the frame in soft, flowing streaks."
                  data-nosnippet="true" loading="lazy" decoding="async" data-nimg="fill"
                  class="object-cover object-center" sizes="(min-width: 1728px) 1728px, 100vw"
                  srcset="https://images.ctfassets.net/kftzwdyauwt9/5q3iK91iYCslMpYW0fmPNc/50776ce6fc897eacb94d2c05533dba96/oai_GA_Stories_16.9.png?w=640&amp;q=90&amp;fm=webp 640w, https://images.ctfassets.net/kftzwdyauwt9/5q3iK91iYCslMpYW0fmPNc/50776ce6fc897eacb94d2c05533dba96/oai_GA_Stories_16.9.png?w=750&amp;q=90&amp;fm=webp 750w, https://images.ctfassets.net/kftzwdyauwt9/5q3iK91iYCslMpYW0fmPNc/50776ce6fc897eacb94d2c05533dba96/oai_GA_Stories_16.9.png?w=828&amp;q=90&amp;fm=webp 828w, https://images.ctfassets.net/kftzwdyauwt9/5q3iK91iYCslMpYW0fmPNc/50776ce6fc897eacb94d2c05533dba96/oai_GA_Stories_16.9.png?w=1080&amp;q=90&amp;fm=webp 1080w, https://images.ctfassets.net/kftzwdyauwt9/5q3iK91iYCslMpYW0fmPNc/50776ce6fc897eacb94d2c05533dba96/oai_GA_Stories_16.9.png?w=1200&amp;q=90&amp;fm=webp 1200w, https://images.ctfassets.net/kftzwdyauwt9/5q3iK91iYCslMpYW0fmPNc/50776ce6fc897eacb94d2c05533dba96/oai_GA_Stories_16.9.png?w=1920&amp;q=90&amp;fm=webp 1920w, https://images.ctfassets.net/kftzwdyauwt9/5q3iK91iYCslMpYW0fmPNc/50776ce6fc897eacb94d2c05533dba96/oai_GA_Stories_16.9.png?w=2048&amp;q=90&amp;fm=webp 2048w, https://images.ctfassets.net/kftzwdyauwt9/5q3iK91iYCslMpYW0fmPNc/50776ce6fc897eacb94d2c05533dba96/oai_GA_Stories_16.9.png?w=3840&amp;q=90&amp;fm=webp 3840w"
                  src="https://images.ctfassets.net/kftzwdyauwt9/5q3iK91iYCslMpYW0fmPNc/50776ce6fc897eacb94d2c05533dba96/oai_GA_Stories_16.9.png?w=3840&amp;q=90&amp;fm=webp">
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div></div>
  <div class="pt-2xl @md:w-full grid grid-cols-12 w-full">
    <div class="@md:col-span-6 @md:col-start-4 pt-3xs border-t-primary-4 col-span-12 flex w-full items-center justify-between border-t-[1px]">
      <div class="flex-col">
        <div class="relative flex">
          <div class="flex items-center">
            <button type="button" class="text-primary-100 bg-primary-4 focus:outline-primary-12 backdrop-blur-[4.375rem] transition duration-200 ease-curve-a flex items-center justify-center disabled:text-gray-40 focus-visible:outline focus-visible:outline-1 outline-offset-2 focus-visible:outline-offset-0 rounded-full w-[32px] h-[32px] hover:bg-primary-12 p-6xs relative shrink-0 grow-0"
            aria-label="Play audio of page text">
              <svg class="translate-x-[8%] transform" xmlns="http://www.w3.org/2000/svg"
              width="11" viewBox="0 0 9 16" fill="none">
                <path d="M0 11.9523V4.04773C0 3.22232 0.911256 2.72209 1.60763 3.16523L7.81833 7.1175C8.46426 7.52854 8.46426 8.47146 7.81833 8.8825L1.60763 12.8348C0.911255 13.2779 0 12.7777 0 11.9523Z"
                fill="currentColor"></path>
              </svg>
            </button>
            <span class="pl-3xs text-cta shrink grow">
              <div class="gap-3xs flex items-center">
                <span>Listen to article</span>
                <div class="border-l-primary-4 py-5xs pl-3xs border-l-[1px] tabular-nums">8:10</div>
              </div>
            </span>
          </div>
        </div>
      </div>
      <div class="ml-auto">
        <div class="relative">
          <div class="gap-5xs flex items-center" type="button" aria-haspopup="dialog"
          aria-expanded="false" aria-controls="radix-:R1dkvf9t9svffa:" data-state="closed">
            <span class="text-cta">
              <button type="button" class="transition duration-short ease-curve-a rounded-[2.5rem] text-nowrap min-h-md flex items-center justify-center gap-[0.3em] text-cta focus:outline focus:outline-1 outline-offset-2 h-[2.5rem] text-primary-100 hover:text-primary-60 disabled:text-primary-44 focus:outline-none focus-visible:outline-primary-44 px-0 !rounded">
                <svg class="-rotate-45" width="24" height="17" viewBox="0 0 16 17"
                fill="none" xmlns="http://www.w3.org/2000/svg">
                  <g clip-path="url(#clip0_1356_1880)">
                    <path d="M10.0013 5.24662H12.0013C12.439 5.24662 12.8725 5.33284 13.2769 5.50036C13.6813 5.66787 14.0488 5.9134 14.3583 6.22293C14.6679 6.53246 14.9134 6.89992 15.0809 7.30434C15.2484 7.70876 15.3346 8.14221 15.3346 8.57995C15.3346 9.01769 15.2484 9.45115 15.0809 9.85556C14.9134 10.26 14.6679 10.6274 14.3583 10.937C14.0488 11.2465 13.6813 11.492 13.2769 11.6596C12.8725 11.8271 12.439 11.9133 12.0013 11.9133H10.0013M6.0013 11.9133H4.0013C3.56356 11.9133 3.13011 11.8271 2.72569 11.6596C2.32127 11.492 1.95381 11.2465 1.64428 10.937C1.01916 10.3119 0.667969 9.46401 0.667969 8.57995C0.667969 7.6959 1.01916 6.84805 1.64428 6.22293C2.2694 5.59781 3.11725 5.24662 4.0013 5.24662H6.0013"
                    stroke="currentColor" stroke-width="1.66667" stroke-linecap="round"
                    stroke-linejoin="round"></path>
                    <path d="M5.33203 8.57996H10.6654" stroke="currentColor"
                    stroke-width="1.66667" stroke-linecap="round" stroke-linejoin="round"></path>
                  </g>
                </svg>Share</button>
            </span>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
<div class="@container max-w-container multi-columns:px-0 multi-columns:flex grid w-full grid-cols-12">
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-sm">
    <p class="mb-sm last:mb-0">At OpenAI, we’re working hard to make AI systems more useful and reliable.
      Even as language models become more capable, one challenge remains stubbornly
      hard to fully solve: hallucinations. By this we mean instances where a model
      confidently generates an answer that isn’t true. Our
      <span>&nbsp;</span><a href="https://cdn.openai.com/pdf/d04913be-3f6f-4d2b-b283-ff432ef4aaa5/why-language-models-hallucinate.pdf"
      class="transition ease-curve-a duration-250 text-primary-100 hover:text-primary-60 relative underline-offset-[0.25rem] decoration-1 underline"
      target="_blank" referrerpolicy="no-referrer-when-downgrade">new research paper⁠<span class="sr-only">(opens in a new window)</span></a>
      <span>&nbsp;</span>argues that language models hallucinate because standard training
      and evaluation procedures reward guessing over acknowledging uncertainty.</p>
  </div>
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-sm">
    <p class="mb-sm last:mb-0">ChatGPT also hallucinates. GPT‑5 has significantly fewer hallucinations
      <span>&nbsp;</span><a class="transition ease-curve-a duration-250 text-primary-100 hover:text-primary-60 relative underline-offset-[0.25rem] decoration-1 underline"
      href="https://openai.com/index/introducing-gpt-5/#:~:text=Building%20a%20more%20robust%2C%20reliable%2C%20and%20helpful%20model">especially when reasoning⁠</a>,
      but they still occur. Hallucinations remain a fundamental challenge for all
      large language models, but we are working hard to further reduce them.</p>
  </div>
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-xl">
    <div class="@container max-w-container grid w-full grid-cols-12 toc-content-heading scroll-mt-[calc(var(--header-h)+var(--toc-button-h))]"
    id="what-are-hallucinations">
      <div class="@md:col-span-6 @md:col-start-4 full-grid-content:@md:col-span-12 full-grid-content:@md:col-start-1 col-span-12 max-w-none">
        <h2 class="text-h3 scroll-mt-[calc(var(--header-h)+var(--toc-button-h))]">What are hallucinations?</h2>
      </div>
    </div>
  </div>
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-sm">
    <p class="mb-sm last:mb-0">Hallucinations are plausible but false statements generated by language models.
      They can show up in surprising ways, even for seemingly straightforward questions.
      For example, when we asked a widely used chatbot for the title of the PhD
      dissertation by Adam Tauman Kalai (an author of this paper), it confidently
      produced three different answers—none of them correct. When we asked for
      his birthday, it gave three different dates, likewise all wrong.&nbsp;</p>
  </div>
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-xl">
    <div class="@container max-w-container grid w-full grid-cols-12 toc-content-heading scroll-mt-[calc(var(--header-h)+var(--toc-button-h))]"
    id="teaching-to-the-test">
      <div class="@md:col-span-6 @md:col-start-4 full-grid-content:@md:col-span-12 full-grid-content:@md:col-start-1 col-span-12 max-w-none">
        <h2 class="text-h3 scroll-mt-[calc(var(--header-h)+var(--toc-button-h))]">Teaching to the test</h2>
      </div>
    </div>
  </div>
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-sm">
    <p class="mb-sm last:mb-0">Hallucinations persist partly because current evaluation methods set the wrong
      incentives. While evaluations themselves do not directly cause hallucinations,
      most evaluations measure model performance in a way that encourages guessing
      rather than honesty about uncertainty.</p>
  </div>
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-sm">
    <p class="mb-sm last:mb-0">Think about it like a multiple-choice test. If you do not know the answer but
      take a wild guess, you might get lucky and be right. Leaving it blank guarantees
      a zero. In the same way, when models are graded only on accuracy, the percentage
      of questions they get exactly right, they are encouraged to guess rather
      than say “I don’t know.”</p>
  </div>
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-sm">
    <p class="mb-sm last:mb-0">As another example, suppose a language model is asked for someone’s birthday
      but doesn’t know. If it guesses “September 10,” it has a 1-in-365 chance
      of being right. Saying “I don’t know” guarantees zero points. Over thousands
      of test questions, the guessing model ends up looking better on scoreboards
      than a careful model that admits uncertainty.</p>
  </div>
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-sm">
    <p class="mb-sm last:mb-0">For questions where there is a single “right answer,” one can consider three
      categories of responses: accurate responses, errors, and abstentions where
      the model does not hazard a guess. Abstaining is part of
      <span>&nbsp;</span><b>humility</b>, one of
      <span>&nbsp;</span><a class="transition ease-curve-a duration-250 text-primary-100 hover:text-primary-60 relative underline-offset-[0.25rem] decoration-1 underline"
      href="https://openai.com/careers/#:~:text=to%20elevate%20humanity.-,Act%20with%20humility.,-Humility%20reminds%20us">OpenAI’s core values⁠</a>.
      Most scoreboards prioritize and rank models based on accuracy, but errors
      are worse than abstentions. Our
      <span>&nbsp;</span><a href="https://model-spec.openai.com/2025-02-12.html#express_uncertainty"
      class="transition ease-curve-a duration-250 text-primary-100 hover:text-primary-60 relative underline-offset-[0.25rem] decoration-1 underline"
      target="_blank" referrerpolicy="no-referrer-when-downgrade">Model Spec⁠<span class="sr-only">(opens in a new window)</span></a>
      <span>&nbsp;</span>states that it is better to indicate uncertainty or ask for
      clarification than provide confident information that may be incorrect.&nbsp;</p>
  </div>
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-sm">
    <p class="mb-sm last:mb-0">For a concrete example, consider the
      <span>&nbsp;</span><a class="transition ease-curve-a duration-250 text-primary-100 hover:text-primary-60 relative underline-offset-[0.25rem] decoration-1 underline"
      href="https://openai.com/index/introducing-simpleqa/">SimpleQA eval</a>
      <span>&nbsp;</span>as an example from the
      <span>&nbsp;</span><a href="https://cdn.openai.com/gpt-5-system-card.pdf" class="transition ease-curve-a duration-250 text-primary-100 hover:text-primary-60 relative underline-offset-[0.25rem] decoration-1 underline"
      target="_blank" referrerpolicy="no-referrer-when-downgrade">GPT5 System Card⁠<span class="sr-only">(opens in a new window)</span></a>.</p>
  </div>
  <div class="col-span-12 [&amp;:not(:first-child)]:mt-sm">
    <div class="max-w-container @container multi-columns:px-0 grid w-full grid-cols-12">
      <div class="full-grid-content:@md:col-span-12 full-grid-content:@md:col-start-1 col-span-12 @md:col-span-6 @md:col-start-4">
        <h5 class="text-h5-mobile @md:text-h5-desktop text-nowrap"></h5>
        <div class="col-span-12 w-full overflow-auto">
          <div class="py-3xs @2xl:[&amp;_table]:table-fixed [&amp;_td]:p-3xs [&amp;_th]:p-4xs [&amp;_td]:min-w-3xl prose max-w-none [&amp;_table]:w-full [&amp;_table]:table-auto [&amp;_table]:border-collapse [&amp;_table]:text-left">
            <div class="scrollable">
              <div class="relative min-w-fit">
                <div class="pointer-events-none absolute bottom-0 left-0 top-0 z-[1] w-[1px]"></div>
                <table>
                  <tbody>
                    <tr class="border-primary-12 border-t-[1px] last:border-b-[1px]">
                      <td class="[&amp;>p]:text-p2 [&amp;>p]:break-words [&amp;>p]:font-semibold">
                        <p><b>Metric</b>
                        </p>
                      </td>
                      <td class="[&amp;>p]:text-p2 [&amp;>p]:break-words [&amp;>p]:font-semibold">
                        <p><b>gpt-5-thinking-mini</b>
                        </p>
                      </td>
                      <td class="[&amp;>p]:text-p2 [&amp;>p]:break-words [&amp;>p]:font-semibold">
                        <p><b>OpenAI o4-mini</b>
                        </p>
                      </td>
                    </tr>
                    <tr class="border-primary-12 border-t-[1px] last:border-b-[1px]">
                      <td class="[&amp;_p]:text-p2 [&amp;>p]:break-words">
                        <p>Abstention rate
                          <br>(no specific answer is given)&nbsp;</p>
                      </td>
                      <td class="[&amp;_p]:text-p2 [&amp;>p]:break-words">
                        <p>52%</p>
                      </td>
                      <td class="[&amp;_p]:text-p2 [&amp;>p]:break-words">
                        <p>1%</p>
                      </td>
                    </tr>
                    <tr class="border-primary-12 border-t-[1px] last:border-b-[1px]">
                      <td class="[&amp;_p]:text-p2 [&amp;>p]:break-words">
                        <p>Accuracy rate
                          <br>(right answer, higher is better)</p>
                      </td>
                      <td class="[&amp;_p]:text-p2 [&amp;>p]:break-words">
                        <p>22%</p>
                      </td>
                      <td class="[&amp;_p]:text-p2 [&amp;>p]:break-words">
                        <p>24%</p>
                      </td>
                    </tr>
                    <tr class="border-primary-12 border-t-[1px] last:border-b-[1px]">
                      <td class="[&amp;_p]:text-p2 [&amp;>p]:break-words">
                        <p>Error rate
                          <br>(wrong answer, lower is better)</p>
                      </td>
                      <td class="[&amp;_p]:text-p2 [&amp;>p]:break-words">
                        <p>26%</p>
                      </td>
                      <td class="[&amp;_p]:text-p2 [&amp;>p]:break-words">
                        <p>75%</p>
                      </td>
                    </tr>
                    <tr class="border-primary-12 border-t-[1px] last:border-b-[1px]">
                      <td class="[&amp;_p]:text-p2 [&amp;>p]:break-words">
                        <p>Total</p>
                      </td>
                      <td class="[&amp;_p]:text-p2 [&amp;>p]:break-words">
                        <p>100%</p>
                      </td>
                      <td class="[&amp;_p]:text-p2 [&amp;>p]:break-words">
                        <p>100%</p>
                      </td>
                    </tr>
                  </tbody>
                </table>
                <div class="pointer-events-none absolute bottom-0 right-0 top-0 w-[1px]"></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-sm">
    <p class="mb-sm last:mb-0">In terms of accuracy, the older OpenAI o4-mini model performs slightly better.
      However, its error rate (i.e., rate of hallucination) is significantly higher.
      Strategically guessing when uncertain improves accuracy but increases errors
      and hallucinations.&nbsp;</p>
  </div>
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-sm">
    <p class="mb-sm last:mb-0">When averaging results across dozens of evaluations, most benchmarks pluck
      out the accuracy metric, but this entails a false dichotomy between right
      and wrong. On simplistic evals like SimpleQA, some models achieve near 100%
      accuracy and thereby eliminate hallucinations. However, on more challenging
      evaluations and in real use, accuracy is capped below 100% because there
      are some questions whose answer cannot be determined for a variety of reasons
      such as unavailable information, limited thinking abilities of small models,
      or ambiguities that need to be clarified.</p>
  </div>
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-sm">
    <p class="mb-sm last:mb-0">Nonetheless, accuracy-only scoreboards dominate leaderboards and model cards,
      motivating developers to build models that guess rather than hold back. That
      is one reason why, even as models get more advanced, they can still hallucinate,
      confidently giving wrong answers instead of acknowledging uncertainty.</p>
  </div>
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-xl">
    <div class="@container max-w-container grid w-full grid-cols-12 scroll-mt-[calc(var(--header-h)+var(--toc-button-h))]"
    id="a-better-way-to-grade-evaluations">
      <div class="@md:col-span-6 @md:col-start-4 full-grid-content:@md:col-span-12 full-grid-content:@md:col-start-1 col-span-12 max-w-none">
        <h4 class="text-h4 scroll-mt-[calc(var(--header-h)+var(--toc-button-h))]">A better way to grade evaluations</h4>
      </div>
    </div>
  </div>
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-sm">
    <p class="mb-sm last:mb-0">There is a straightforward fix. Penalize confident errors more than you penalize
      uncertainty, and give partial credit for appropriate expressions of uncertainty.
      This idea is not new. Some standardized tests have long used versions of
      negative marking for wrong answers or partial credit for leaving questions
      blank to discourage blind guessing. Several research groups have also explored
      evaluations that account for uncertainty and calibration.</p>
  </div>
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-sm">
    <p class="mb-sm last:mb-0">Our point is different. It is not enough to add a few new uncertainty-aware
      tests on the side. The widely used, accuracy-based evals need to be updated
      so that their scoring discourages guessing. If the main scoreboards keep
      rewarding lucky guesses, models will keep learning to guess. Fixing scoreboards
      can broaden adoption of hallucination-reduction techniques, both newly developed
      and those from prior research.</p>
  </div>
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-xl">
    <div class="@container max-w-container grid w-full grid-cols-12 toc-content-heading scroll-mt-[calc(var(--header-h)+var(--toc-button-h))]"
    id="how-hallucinations-originate-from-next-word-prediction">
      <div class="@md:col-span-6 @md:col-start-4 full-grid-content:@md:col-span-12 full-grid-content:@md:col-start-1 col-span-12 max-w-none">
        <h2 class="text-h3 scroll-mt-[calc(var(--header-h)+var(--toc-button-h))]">How hallucinations originate from next-word prediction</h2>
      </div>
    </div>
  </div>
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-sm">
    <p class="mb-sm last:mb-0">We’ve talked about why hallucinations are so hard to get rid of, but where
      do these highly-specific factual inaccuracies come from in the first place?
      After all, large pretrained models rarely exhibit other kinds of errors such
      as spelling mistakes and mismatched parentheses. The difference has to do
      with what kinds of patterns there are in the data.</p>
  </div>
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-sm">
    <p class="mb-sm last:mb-0">Language models first learn through
      <span>&nbsp;</span><i>pretraining</i>, a process of predicting the next word in
      huge amounts of text. Unlike traditional machine learning problems, there
      are no “true/false” labels attached to each statement. The model sees only
      positive examples of fluent language and must approximate the overall distribution.&nbsp;</p>
  </div>
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-sm">
    <p class="mb-sm last:mb-0">It’s doubly hard to distinguish valid statements from invalid ones when you
      don’t have any examples labeled as invalid. But even with labels, some errors
      are inevitable. To see why, consider a simpler analogy. In image recognition,
      if millions of cat and dog photos are labeled as “cat” or “dog,” algorithms
      can learn to classify them reliably. But imagine instead labeling each pet
      photo by the pet’s birthday. Since birthdays are essentially random, this
      task would always produce errors, no matter how advanced the algorithm.</p>
  </div>
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-sm">
    <p class="mb-sm last:mb-0">The same principle applies in pretraining. Spelling and parentheses follow
      consistent patterns, so errors there disappear with scale. But arbitrary
      low-frequency facts, like a pet’s birthday, cannot be predicted from patterns
      alone and hence lead to hallucinations. Our analysis explains which kinds
      of hallucinations should arise from next-word prediction. Ideally, further
      stages after pretraining should remove them, but this is not fully successful
      for reasons described in the previous section.&nbsp;</p>
  </div>
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-xl">
    <div class="@container max-w-container grid w-full grid-cols-12 toc-content-heading scroll-mt-[calc(var(--header-h)+var(--toc-button-h))]"
    id="conclusions">
      <div class="@md:col-span-6 @md:col-start-4 full-grid-content:@md:col-span-12 full-grid-content:@md:col-start-1 col-span-12 max-w-none">
        <h2 class="text-h3 scroll-mt-[calc(var(--header-h)+var(--toc-button-h))]">Conclusions</h2>
      </div>
    </div>
  </div>
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-sm">
    <p class="mb-sm last:mb-0">We hope that the statistical lens in our paper clarifies the nature of hallucinations
      and pushes back on common misconceptions:</p>
  </div>
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-sm">
    <ul class="mb-md marker:text-inherit last:mb-0 list-disc pl-2xs mx-3xs">
      <li class="mb-4xs last:mb-0"><b>Claim:</b>
        <span>&nbsp;</span>Hallucinations will be eliminated by improving accuracy because
        a 100% accurate model never hallucinates.<b><br>Finding:<span>&nbsp;</span></b>Accuracy
        will never reach 100% because, regardless of model size, search and reasoning
        capabilities,<b><span>&nbsp;</span></b>some real-world questions are inherently
        unanswerable.&nbsp;</li>
      <li class="mb-4xs last:mb-0"><b>Claim:<span>&nbsp;</span></b>Hallucinations are inevitable.<b><br>Finding:</b>
        <span>&nbsp;</span>They are not, because language models can abstain when uncertain.</li>
      <li
      class="mb-4xs last:mb-0"><b>Claim:</b>
        <span>&nbsp;</span>Avoiding hallucinations requires a degree of intelligence
        which is exclusively achievable with larger models.<b><br>Finding:</b>
        <span>&nbsp;</span>It can be
        <span>&nbsp;</span><i>easier</i>
        <span>&nbsp;</span>for a small model to know its limits. For example, when asked
        to answer a Māori question, a small model which knows no Māori can simply
        say “I don’t know” whereas a model that knows some Māori has to determine
        its confidence. As discussed in the paper, being “calibrated” requires
        much less computation than being accurate.</li>
        <li class="mb-4xs last:mb-0"><b>Claim:<span>&nbsp;</span></b>Hallucinations are a mysterious glitch
          in modern language models.<b><br>Finding:<span>&nbsp;</span></b>We understand
          the statistical mechanisms through which hallucinations arise and are
          rewarded in evaluations.</li>
        <li class="mb-4xs last:mb-0"><b>Claim:<span>&nbsp;</span></b>To measure hallucinations, we just need
          a good hallucination eval.<b><br>Finding:<span>&nbsp;</span></b>Hallucination
          evals have been published. However, a good hallucination eval has little
          effect against hundreds of traditional accuracy-based evals that penalize
          humility and reward guessing. Instead, all of the primary eval metrics
          need to be reworked to reward expressions of uncertainty.</li>
    </ul>
  </div>
  <div class="@md:col-span-6 @md:col-start-4 col-span-12 max-w-none [&amp;:not(:first-child)]:mt-sm">
    <p class="mb-sm last:mb-0">Our latest models have lower hallucination rates, and we continue to work hard
      to further decrease the rates of confident errors output by our language
      models.</p>
  </div>
</div>
<!--EndFragment-->

<!--EndFragment-->