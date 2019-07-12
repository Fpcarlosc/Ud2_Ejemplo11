# Ud2_Ejemplo11
_Ejemplo 11 de la Unidad 2._ 

Vemos un ejemplo de uso de ScrollView sobre ConstraintLayout. Para ello se ha escalado una imagen de tal forma que no quepa en la pantalla y se necesite hacer _scroll_ para verla entera.

Sólo hemos de fijarnos en el fichero _activity_main.xml_:

```
<ScrollView xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <android.support.constraint.ConstraintLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent">

        <ImageView
            android:layout_width="100dp"
            android:layout_height="2000dp"
            android:scaleType="centerCrop"
            android:src="@drawable/grand_canyon"

            app:layout_constraintBottom_toBottomOf="parent"
            app:layout_constraintLeft_toLeftOf="parent"
            app:layout_constraintRight_toRightOf="parent"
            app:layout_constraintTop_toTopOf="parent" />

    </android.support.constraint.ConstraintLayout>
</ScrollView>
```

Observad que el espacio de nombres ahora está en en la definición de _ScrollView_ y no en la de _ConstraintLayout_.

_Imagen de Pixabay.com (Licencia CC0)_
