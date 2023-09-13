# quadratic-form-conversion
Convert quadratics from Homogeneous to Center form and back.

This zip file contains 2 functions to transform generic (nD) quadratic hyper-surfaces from homogeneous form (that is [x' 1]*E*[x;1]=0) to center form (that is (x'-c')*inv(Q)*(x-c)=1, which is used for example in the ellipsoidal toolbox).

Examples:
% zero-centered ellipse of semiaxes 1 and 2
% center to homogeneous form:
E=c2h(diag([1 4]),[0 0]')
% homogeneous to center form:
[Q,c]=h2c(E)
