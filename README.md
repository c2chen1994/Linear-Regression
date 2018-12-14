# Linear-Regression

	Problem 1.1 Linear regression
		Implement linear regression and return the model parameters.
			function linear_regression_noreg(X, y).

	Problem 1.2 Regularized linear regression
		To prevent overfitting, we usually add regularization. For now, we will focus on L2 regularization. In
		this case, the optimization problem is:
			w(lambda) = argmin(w)||Xw - y||2 + lambda||w||2
		where lambda is a hyper-parameter used to control the complexity of the resulting model. When lambda = 0,
		the model reduces to the usual (unregularized) linear regression. For lambda > 0 the objective function balances
		between two terms: (1) the data-dependent quadratic loss function ||Xw - y||2,
		and (2) a function of the model parameters ||w||2.
		
		Implement the regularized linear regression algorithm.
			function regularized_linear+regression(X, y, lambda).

	Problem 1.3 Tuning the regularization hyper-parameter
		Use the validation set to tune the regularization parameter lambda: {0, 10-4, 10-3, 10-2, 10-1, 1, 10, 102}. We
		select the best one that results in the lowest mean square error on the validation set.
			function tune_lambda(Xtrain, ytrain, Xval, yval, lambds).

	Problem 1.4 Mean square error
		Report the mean square error of the model on the give n test set.
			function test_error(w, X, y).