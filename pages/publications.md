---
layout: page
---

Thesis

- Abstraction via Program Transformation (_doctoral thesis_)
  <div id="doctoral-materials">
    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#abstract-doctoral" aria-expanded="false" aria-controls="abstract-doctoral">
    Abstract
    </button>

    <button class="btn btn-link" type="button">
    <a href="https://is.muni.cz/th/mkjtn/?lang=en">Web</a>
    </button>

    <div class="collapse" id="abstract-doctoral">
      <hr>
      In the field of computer-aided verification, abstraction techniques are indispensable as they play a critical role in reducing the complexity of the verification process to manageable sizes. However, these techniques are usually tightly integrated into tools, resulting in undesired complexity and neglect of reusable design. If one wants to employ a particular abstraction in several tools, the common approach is to implement the abstraction separately for each tool. However, this results in unnecessary duplication of an effort and inconsistent results as different implementations may vary. This thesis aims to address this challenge by developing a solution to reduce the duplication and complexity of abstraction. The overarching objective is to create a tool-independent program abstraction and utilize it to design program analysis techniques that can be applied by any tool, thereby reducing its complexity and allowing abstraction reusability. What is common between tools is the program representation they operate with. One such representation that has gained popularity is the LLVM intermediate representation of the Clang compiler. It can serve as a shared source of truth between tools and encode additional information for program analysis. In this doctoral thesis, we propose a solution to tool-independent abstraction by reconceiving it in terms of the intermediate representation. The key idea of the presented approach is to express abstract semantics in terms of intermediate representation, resulting in the abstraction being understandable to any tool which uses LLVM IR. We refer to this approach as compilation-based abstraction, as it essentially compiles abstract semantics into the program being analyzed. The compilation-based abstraction approach has broad applicability in the field of program analysis. This thesis demonstrates its potential in recasting symbolic execution as program abstraction, enabling explicit tools to perform symbolic analysis or even run symbolic programs natively. The focus will also be on more complex program primitives such as C arrays or strings, which require elaborated abstraction. The approach is extended to encompass aggregate types and library-level abstractions. Additionally, attention is given to dynamic memory abstraction, specifically the problem of ambiguous dynamic memory layout, which is often overlooked in analysis tools. Furthermore, the compilation-based abstraction approach opens up new possibilities for refinement techniques that can enhance the precision of the employed abstraction. This thesis explores the potential for instrumenting refinement directly into the program and counterexample-guided syntactic abstraction of program representation. In summary, this thesis provides an autonomous solution for instrumenting abstraction into program representation. The presented approach addresses various issues related to program domain interactions, control flow, and dynamic memory. It includes adaptations of symbolic execution, software model checking, and syntactic refinement loops. Moreover, by enabling the native execution of compiled abstraction, this approach not only streamlines the program abstraction design process but also enhances the efficiency of program analysis. Our main contributions culminated in the development of an LLVM Abstraction & Refinement Tool – LART. This tool implements all discussed abstractions and has been shown to be effective both in conjunction with other tools and in producing natively executable abstractions.
      <hr>
    </div>
  </div>

- Abstractions via Program Transformations (_advanced master thesis_)
  <div id="amaster-materials">
    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#abstract-amaster" aria-expanded="false" aria-controls="abstract-amaster">
    Abstract
    </button>

    <button class="btn btn-link" type="button">
    <a href="https://is.muni.cz/th/uqf69/?lang=en">Web</a>
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
    <a href="https://is.muni.cz/th/owq0x/?lang=en">Web</a>
    </button>

    <div class="collapse" id="abstract-master">
      <hr>
      To show reliability of software, developers usually reach out for testing and static analysis. However, to prove correctness, all behaviours of a program need to be checked. In this respect, formal verification methods aim to provide an automated approach to verification. A big obstacle are inputs because they massively increase the number of behaviours of the program. In this thesis, we present a technique which enables verification tools to perform automated checking of programs with inputs. A generally known approach is to interpret operations with input values in an abstract way. In this case, abstraction needs to be implemented in the verification tool. We propose that instead, an abstraction can be compiled into the program. Hence, the program can be verified by a tool even though the tool itself does not support abstraction of inputs. We implement the proposed approach as an LLVM-to-LLVM transformation which inserts an abstraction to the program. The applicability of the approach is demonstrated by transforming programs to represent their inputs symbolically. This, in turn, enables an essentially explicit-state model checker to verify the program. For evaluation purposes, we have chosen DIVINE as the model checker.
      <hr>
    </div>
    <i class='fa fa-trophy'> Dean's award for an Outstanding Final Thesis</i>
  </div>


- Introduction to Data Structures in Examples (_bachelor thesis_)
  <div id="bachelor-materials">
    <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#abstract-bachelor" aria-expanded="false" aria-controls="abstract-bachelor">
    Abstract
    </button>

    <button class="btn btn-link" type="button">
    <a href="https://is.muni.cz/th/vlg4z/?lang=en">Web</a>
    </button>

    <div class="collapse" id="abstract-bachelor">
      <hr>
      This thesis presents methods and structures proposed for teaching and home study of data structures. The thesis describes creation process of concrete exercises and their solutions. A part of exercises cover practical implementations, that contains code templates to be solved and a package of tests. Themes covered in the thesis are elementary data structures such as stack, queue, linked list and their modifications. Moreover, the thesis covers dynamic data structures for searching: binary heap, searching trees, red-black trees and B-trees. The thesis also comprehends data structures for the implementation of dictionaries.
    </div>
  </div>

---


{% for year in (2016..2022) reversed %}

{{ year }}
{% bibliography --query @*[year={{ year }}] %}

{% if forloop.last == false %}
  ---
{% endif %}

{% endfor %}
