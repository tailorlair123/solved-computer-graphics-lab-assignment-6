Download Link: https://assignmentchef.com/product/solved-computer-graphics-lab-assignment-6
<br>
<strong>Computer Graphics, Lab Assignment 6 </strong>




+ LabAssignment2/

+ 1/

<ul>

 <li>py</li>

</ul>

+ 2/

<ul>

 <li>py</li>

</ul>

+ 3/

<ul>

 <li>py</li>

</ul>




<ul>

 <li>The submission time is determined not when the commit is made but when the git push is made.</li>

</ul>




<ol>

 <li>Write your own myLookAt() and myOrtho() functions (of the following form) that behaves exactly same as gluLookAt() and glOrtho().</li>

</ol>

<strong>def</strong> myLookAt<strong>(</strong>eye<strong>,</strong> at<strong>,</strong> up<strong>): </strong># eye, at, up are 1D numpy array of length 3 <strong>def</strong> myOrtho<strong>(</strong>left<strong>,</strong> right<strong>,</strong> bottom<strong>,</strong> top<strong>,</strong> zNear<strong>,</strong> zFar<strong>):</strong>

<ol>

 <li></li>

 <li>Set the window title to <strong>your student ID</strong> and the window size to (480,480).</li>

 <li>Code skeleton</li>

 <li>Find code for drawFrame(), drawCubeArray() from 6-Viewing,Projection</li>

 <li><strong>DO NOT use gluLookAt() inside myLookAt() and glOrtho() inside myOrtho()! </strong></li>

 <li>Your program should render the following scene:</li>

 <li></li>

 <li>Hint:

  <ol>

   <li>Everything you need to write code is in 6-Viewing,Projection</li>

   <li>l2 norm of <strong>v</strong> : ||<strong>v</strong>|| = np.sqrt( np.dot(<strong>v</strong>, <strong>v</strong>) )</li>

   <li><strong>a</strong> x <strong>b </strong>(cross product) : np.cross(<strong>a</strong>, <strong>b</strong>)</li>

   <li><strong>a</strong> ∙ <strong>b</strong> (inner product) : np.dot(<strong>a</strong>, <strong>b</strong>) or <strong>a</strong>@<strong>b</strong></li>

   <li>Use glMultMatrixf() to multiply your projection matrix and viewing matrix to the current transformation matrix.</li>

  </ol></li>

 <li>Files to submit: A Python source file (Name the file whatever you want (in English). Extension should be .py)</li>

</ol>




<ol start="2">

 <li>As mentioned in the lecture, “moving camera” and “moving world” are two equivalent operations. Based on the following figure, replace the gluLookAt call() in the following code with <strong>two glRotatef() calls and one glTranslatef() call</strong> and complete the program.</li>

</ol>

<table width="583">

 <tbody>

  <tr>

   <td width="583">

    <table width="427">

     <tbody>

      <tr>

       <td width="104"><strong>def</strong> render<strong>():</strong></td>

       <td colspan="4" width="323"> </td>

      </tr>

      <tr>

       <td colspan="5" width="427">    glClear<strong>(</strong>GL_COLOR_BUFFER_BIT <strong>|</strong> GL_DEPTH_BUFFER_BIT<strong>)</strong></td>

      </tr>

      <tr>

       <td colspan="3" width="211">    glEnable<strong>(</strong>GL_DEPTH_TEST<strong>)</strong></td>

       <td colspan="2" width="216"> </td>

      </tr>

      <tr>

       <td colspan="4" width="371">    glPolygonMode<strong>(</strong> GL_FRONT_AND_BACK<strong>,</strong> GL_LINE <strong>)</strong></td>

       <td rowspan="2" width="56"> </td>

      </tr>

      <tr>

       <td colspan="2" width="155">    glLoadIdentity<strong>()</strong></td>

       <td colspan="2" width="216"> </td>

      </tr>

      <tr>

       <td width="104"></td>

       <td width="51"></td>

       <td width="56"></td>

       <td width="160"></td>

       <td width="56"></td>

      </tr>

     </tbody>

    </table> gluPerspective<strong>(</strong>45<strong>,</strong> 1<strong>,</strong> 1<strong>,</strong>10<strong>)</strong> <strong># Replace this call with </strong><strong>two glRotatef() calls and one glTranslatef() call </strong><strong>    gluLookAt</strong><strong>(</strong><strong>3</strong><strong>,</strong><strong>3</strong><strong>,</strong><strong>3</strong><strong>,</strong> <strong>0</strong><strong>,</strong><strong>0</strong><strong>,</strong><strong>0</strong><strong>,</strong> <strong>0</strong><strong>,</strong><strong>1</strong><strong>,</strong><strong>0</strong><strong>)</strong> drawFrame<strong>()</strong>


    <table width="227">

     <tbody>

      <tr>

       <td colspan="2" width="227">    glColor3ub<strong>(</strong>255<strong>,</strong> 255<strong>,</strong> 255<strong>)</strong></td>

      </tr>

      <tr>

       <td width="147">    drawCubeArray<strong>()</strong></td>

       <td width="80"> </td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<ol>

 <li></li>

 <li></li>

 <li>Set the window title to <strong>your student ID</strong> and the window size to (480,480).</li>

 <li>Find code for drawFrame(), drawCubeArray() from 5-RenderingPipeline slides.</li>

 <li>Your program should render the following scene:</li>

 <li></li>

 <li>Files to submit: A Python source file (Name the file whatever you want (in English). Extension should be .py)</li>

</ol>


