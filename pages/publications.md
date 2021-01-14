---
layout: page
---

Thesis

- Abstractions via Program Transformations (_advanced master thesis_)
  <div id="amaster-materials">
    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#abstract-amaster" aria-expanded="false" aria-controls="abstract-amaster">
    Abstract
    </button>

    <button class="btn btn-link" type="button">
    <a href="https://is.muni.cz/auth/th/uqf69/?lang=en">Web</a>
    </button>

    <div class="collapse" id="abstract-amaster">
      <hr>
      In computer-aided verification, most of the tools leverage abstraction techniques to reduce the complexity of analyzed systems. Even though these techniques are widely adopted, they are usually tightly integrated into tools, causing undesired complexity, and neglect any reusable design. In my research, I focus on the investigation of abstraction-based techniques used in program verification as abstract interpretation, counterexample guided abstraction or symbolic execution. For these techniques, I devise self-contained alternatives and general-purpose analyses. As a solution for self-contained abstraction, I propose a transformation-based method. This method utilizes instrumentation to insert abstraction directly to the program and consequently quits of responsibility for abstraction from the verification tools. Up until now, I have developed transformation-based symbolic execution and string abstraction for explicit model checkers. In the future, I plan to generalize the transformation-based technique for a wider variety of abstract domains such as predicate or pointer abstraction. Furthermore, I intend to adapt traditional abstraction refinement techniques to the self-contained abstraction.
      <hr>
    </div>
  </div>

- Symbolic Model Checking via Program Transformations (_master thesis_)
  <div id="master-materials">
    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#abstract-master" aria-expanded="false" aria-controls="abstract-master">
    Abstract
    </button>

    <button class="btn btn-link" type="button">
    <a href="https://is.muni.cz/auth/th/owq0x/?lang=en">Web</a>
    </button>

    <div class="collapse" id="abstract-master">
      <hr>
      To show reliability of software, developers usually reach out for testing and static analysis. However, to prove correctness, all behaviours of a program need to be checked. In this respect, formal verification methods aim to provide an automated approach to verification. A big obstacle are inputs because they massively increase the number of behaviours of the program. In this thesis, we present a technique which enables verification tools to perform automated checking of programs with inputs. A generally known approach is to interpret operations with input values in an abstract way. In this case, abstraction needs to be implemented in the verification tool. We propose that instead, an abstraction can be compiled into the program. Hence, the program can be verified by a tool even though the tool itself does not support abstraction of inputs. We implement the proposed approach as an LLVM-to-LLVM transformation which inserts an abstraction to the program. The applicability of the approach is demonstrated by transforming programs to represent their inputs symbolically. This, in turn, enables an essentially explicit-state model checker to verify the program. For evaluation purposes, we have chosen DIVINE as the model checker.
      <hr>
    </div>
  </div>


- Introduction to data structures in examples (_bachelor thesis_)
  <div id="bachelor-materials">
    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#abstract-bachelor" aria-expanded="false" aria-controls="abstract-bachelor">
    Abstract
    </button>

    <button class="btn btn-link" type="button">
    <a href="https://is.muni.cz/auth/th/vlg4z/?lang=en">Web</a>
    </button>

    <div class="collapse" id="abstract-bachelor">
      <hr>
      This thesis presents methods and structures proposed for teaching and home study of data structures. The thesis describes creation process of concrete exercises and their solutions. A part of exercises cover practical implementations, that contains code templates to be solved and a package of tests. Themes covered in the thesis are elementary data structures such as stack, queue, linked list and their modifications. Moreover, the thesis covers dynamic data structures for searching: binary heap, searching trees, red-black trees and B-trees. The thesis also comprehends data structures for the implementation of dictionaries.
    </div>
  </div>

---


{% for year in (2016..2020) reversed %}

{{ year }}
{% bibliography --query @*[year={{ year }}] %}

{% if forloop.last == false %}
  ---
{% endif %}

{% endfor %}
