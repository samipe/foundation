<template>
    <div class="row no-gutters">
     <div class="col-md-2">
         <navigation-vertical :pages="pages"/>
     </div>

    <div class="col-md-10" id="scroller"
    ref="content" style="position:relative;height:100vh;overflow-y:scroll;overflow-x:hidden;-webkit-overflow-scrolling: touch;">
        <app-header/>
        <page-block v-for="(page, index) in pages"
          v-bind:page="page"
          v-bind:index="index"
          v-bind:key="index"
          class="pl-md-5 px-lg-2 p-sm-3 py-5 p-xs-1"/>
        <app-footer class="mt-0 py-5"/>
      </div>
    </div>
</template>
<script>
import PageBlock from "@/Components/PageBlock.vue";

export default {
  components: {
    PageBlock
  },
  data() {
    return {
      pages: [
        {
          title: "Who we are",
          text_block: true,
          tab_box: false,
          feature_box: false,
          data: {
            text: {
              twitter: false,
              header: "Who we are",
              text:
                '<p> <b>Robot Framework</b> is a generic open source test automation framework for acceptance testing and acceptance test-driven development (ATDD). For more details about the framework itself see http://robotframework.org. <br><br><b>Robot Framework Foundation</b> is a non-profit consortium that fosters the growth of Robot Framework. It was founded by companies with a common interest to ensure the development of framework now and in the future. </p>'
            }
          }
        },
        {
          title: "What we do",
          text_block: true,
          tab_box: false,
          feature_box: false,
          data: {
            text: {
              twitter: true,
              header: "What we do",
              text:
                '<p> <b>Robot Framework</b> is a generic test automation framework for acceptance testing and acceptance test-driven development (ATDD). It has easy-to-use tabular test data syntax and it utilizes the keyword-driven testing approach. Its testing capabilities can be extended by test libraries implemented either with Python or Java, and users can create new higher-level keywords from existing ones using the same syntax that is used for creating test cases. </p> <p> Robot Framework project is hosted on <a href="https://github.com/robotframework/robotframework" target="_blank">GitHub</a> where you can find further documentation, source code, and issue tracker. Downloads are hosted at <a href="https://pypi.python.org/pypi/robotframework" target="_blank">PyPI</a>. The framework has a rich ecosystem around it consisting of various generic <a href="#libraries">test libraries</a> and <a href="#tools">tools</a> that are developed as separate projects. </p> <p> Robot Framework is operating system and application independent. The core framework is implemented using <a href="http://python.org" target="_blank">Python</a> and runs also on <a href="http://jython.org" target="_blank">Jython</a> (JVM) and <a href="http://ironpython.net" target="_blank">IronPython</a> (.NET). </p> <p> Robot Framework itself is open source software released under <a href="http://www.apache.org/licenses/LICENSE-2.0.html" target="_blank">Apache License 2.0</a>, and most of the libraries and tools in the ecosystem are also open source. The framework was initially developed at <a href="http://networks.nokia.com" target="_blank">Nokia Networks</a> and it is nowadays sponsored by <a href="http://robotframework.org/foundation" target="_blank">Robot Framework Foundation</a>. </p>'
            }
          }
        },
        {
          title: "How to join",
          text_block: true,
          tab_box: false,
          feature_box: false,
          data: {
            text: {
              twitter: true,
              header: "How to join",
              text:
                '<p> <b>Robot Framework</b> is a generic test automation framework for acceptance testing and acceptance test-driven development (ATDD). It has easy-to-use tabular test data syntax and it utilizes the keyword-driven testing approach. Its testing capabilities can be extended by test libraries implemented either with Python or Java, and users can create new higher-level keywords from existing ones using the same syntax that is used for creating test cases. </p> <p> Robot Framework project is hosted on <a href="https://github.com/robotframework/robotframework" target="_blank">GitHub</a> where you can find further documentation, source code, and issue tracker. Downloads are hosted at <a href="https://pypi.python.org/pypi/robotframework" target="_blank">PyPI</a>. The framework has a rich ecosystem around it consisting of various generic <a href="#libraries">test libraries</a> and <a href="#tools">tools</a> that are developed as separate projects. </p> <p> Robot Framework is operating system and application independent. The core framework is implemented using <a href="http://python.org" target="_blank">Python</a> and runs also on <a href="http://jython.org" target="_blank">Jython</a> (JVM) and <a href="http://ironpython.net" target="_blank">IronPython</a> (.NET). </p> <p> Robot Framework itself is open source software released under <a href="http://www.apache.org/licenses/LICENSE-2.0.html" target="_blank">Apache License 2.0</a>, and most of the libraries and tools in the ecosystem are also open source. The framework was initially developed at <a href="http://networks.nokia.com" target="_blank">Nokia Networks</a> and it is nowadays sponsored by <a href="http://robotframework.org/foundation" target="_blank">Robot Framework Foundation</a>. </p>'
            }
          }
        },
        {
          title: "Members",
          text_block: true,
          tab_box: false,
          feature_box: false,
          data: {
            text: {
              twitter: true,
              header: "Who we are",
              text:
                '<p> <b>Robot Framework</b> is a generic test automation framework for acceptance testing and acceptance test-driven development (ATDD). It has easy-to-use tabular test data syntax and it utilizes the keyword-driven testing approach. Its testing capabilities can be extended by test libraries implemented either with Python or Java, and users can create new higher-level keywords from existing ones using the same syntax that is used for creating test cases. </p> <p> Robot Framework project is hosted on <a href="https://github.com/robotframework/robotframework" target="_blank">GitHub</a> where you can find further documentation, source code, and issue tracker. Downloads are hosted at <a href="https://pypi.python.org/pypi/robotframework" target="_blank">PyPI</a>. The framework has a rich ecosystem around it consisting of various generic <a href="#libraries">test libraries</a> and <a href="#tools">tools</a> that are developed as separate projects. </p> <p> Robot Framework is operating system and application independent. The core framework is implemented using <a href="http://python.org" target="_blank">Python</a> and runs also on <a href="http://jython.org" target="_blank">Jython</a> (JVM) and <a href="http://ironpython.net" target="_blank">IronPython</a> (.NET). </p> <p> Robot Framework itself is open source software released under <a href="http://www.apache.org/licenses/LICENSE-2.0.html" target="_blank">Apache License 2.0</a>, and most of the libraries and tools in the ecosystem are also open source. The framework was initially developed at <a href="http://networks.nokia.com" target="_blank">Nokia Networks</a> and it is nowadays sponsored by <a href="http://robotframework.org/foundation" target="_blank">Robot Framework Foundation</a>. </p>'
            }
          }
        },
        {
          title: "Contact info",
          text_block: true,
          tab_box: false,
          feature_box: false,
          data: {
            text: {
              twitter: true,
              header: "Who we are",
              text:
                '<p> <b>Robot Framework</b> is a generic test automation framework for acceptance testing and acceptance test-driven development (ATDD). It has easy-to-use tabular test data syntax and it utilizes the keyword-driven testing approach. Its testing capabilities can be extended by test libraries implemented either with Python or Java, and users can create new higher-level keywords from existing ones using the same syntax that is used for creating test cases. </p> <p> Robot Framework project is hosted on <a href="https://github.com/robotframework/robotframework" target="_blank">GitHub</a> where you can find further documentation, source code, and issue tracker. Downloads are hosted at <a href="https://pypi.python.org/pypi/robotframework" target="_blank">PyPI</a>. The framework has a rich ecosystem around it consisting of various generic <a href="#libraries">test libraries</a> and <a href="#tools">tools</a> that are developed as separate projects. </p> <p> Robot Framework is operating system and application independent. The core framework is implemented using <a href="http://python.org" target="_blank">Python</a> and runs also on <a href="http://jython.org" target="_blank">Jython</a> (JVM) and <a href="http://ironpython.net" target="_blank">IronPython</a> (.NET). </p> <p> Robot Framework itself is open source software released under <a href="http://www.apache.org/licenses/LICENSE-2.0.html" target="_blank">Apache License 2.0</a>, and most of the libraries and tools in the ecosystem are also open source. The framework was initially developed at <a href="http://networks.nokia.com" target="_blank">Nokia Networks</a> and it is nowadays sponsored by <a href="http://robotframework.org/foundation" target="_blank">Robot Framework Foundation</a>. </p>'
            }
          }
        }
      ]
    } 
  }
};
</script>
